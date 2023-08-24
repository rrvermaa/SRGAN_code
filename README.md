# Environment Setup
Open anaconda prompt and cd to the folder where you have your environment.yml file

conda env create -f environment.yml

conda activate srganenv_gpu 


# Train your Model:
!python3 main.py --LR_path custom_dataset/lr_images --GT_path custom_dataset/hr_images

# Test your Model:
!python3 main.py --mode test_only --LR_path test_data/ --generator_path ./model/pre_trained_model_200.pt
