# DreamBooth Reimplementation

This repository contains our reimplementation and experimental exploration of DreamBooth for subject-driven text-to-image generation. Our goal was to understand the main DreamBooth training setup, reproduce its behavior on several subjects, and test how different training choices affected the generated images.

The project includes several notebooks because we ran multiple experiments in parallel. Different notebooks correspond to different subject sets, prompt styles, learning rates, and ablation experiments. For example, some notebooks focus on generating images of specific subjects such as Killian, while others compare different learning rates or test object generation across subjects like dogs, cats, clocks, backpacks, robot toys, plushies, sneakers, and teapots.

The main results are organized in the `Results/` folder. Each experiment has its own folder, and inside each experiment folder there are subfolders for each subject/object. For example:

Results/experiment_name/object_name/

Inside each object folder, the most important file is usually:

grid.png

This image grid shows the final generated outputs for that subject and is the easiest way to visually inspect the result of the experiment. Other useful files are also included, such as:

loss_curve.png
prior_vs_no_prior.png
preview_step_400.png
drift_step_400.png
metrics_table.png
all_metrics.csv

These files help compare training behavior, prompt performance, prior preservation effects, and output quality across experiments.

## Final Submission Files

- Final report: `final_report.pdf`
- Poster: `poster.pdf`

The poster PDF is included in the repository so that the final presentation materials are available along with the code, dataset, and generated results.

## Repository Structure

- `dreambooth_dataset/`
  - Contains the subject images used for training. These include several official/object-style subjects as well as custom subjects used in our experiments.

- `Results/`
  - Contains generated outputs, image grids, loss curves, prior-vs-no-prior comparisons, and metrics for each experiment.

- `*.ipynb`
  - Colab notebooks used to run the experiments. Different notebooks were used for different experiment groups, such as learning rate comparisons, object generation, dog breed mixing, and rich prompt generation.

## Experiments

We ran several types of experiments:

1. Subject generation experiments
   - We trained DreamBooth-style models on different subjects and evaluated whether the model could preserve the subject identity while placing it into new prompts and scenes.

2. Learning rate comparisons
   - We tested different learning rates to see how training stability and output quality changed. Some experiments compare runs such as lower learning rate versus higher learning rate settings.

3. Prior preservation comparisons
   - We compared outputs with and without prior preservation. These results are shown in files such as `prior_vs_no_prior.png`.

4. Prompt variation experiments
   - We tested richer prompts and different prompt styles to see how well the fine-tuned model could generalize beyond simple training-like prompts.

5. Multi-subject/object experiments
   - We tested several object categories and subjects, including animals, toys, household objects, and custom subjects.

## How to View Results

To inspect the results, open the `Results/` folder and choose an experiment folder. Then open the subject/object subfolder and look at:

grid.png

For example:

Results/dog2_cat2_clock_lr5/dog2/grid.png

This will show the generated images for that object under that experiment. For comparisons, open files like:

prior_vs_no_prior.png
loss_curve.png
metrics_table.png

These files summarize how the experiment performed and how the training setup affected the final generations.

## Notes

This project was mainly run through Google Colab notebooks. Because we ran several experiments separately, the repository contains multiple notebooks rather than one single script. Each notebook corresponds to a different experimental direction, such as testing a different subject set, trying a different learning rate, or generating final image grids for analysis.

Overall, the repository is meant to show both the implementation process and the experimental results. The notebooks show how the experiments were run, while the `Results/` folder contains the final outputs used for analysis in our report.
