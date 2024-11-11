# YOLO-Model-Label Changer

This Python script allows you to easily update the class names in a pre-trained YOLO (You Only Look Once) object detection model. The script loads the YOLO model, provides a way to map the existing class names to new ones, and then saves the updated model with the new class names.

## Features

- Load a pre-trained YOLO model from a specified file path
- Display the existing class names in the loaded model
- Provide a dictionary to map the existing class names to new ones
- Update the model's class names with the new mapping
- Save the updated model to a new file

## Usage

1. Clone the repository:

   ```
   git clone https://github.com/SakibAhmedShuva/YOLO-Model-Label-Changer.git
   ```

2. Navigate to the project directory:

   ```
   cd YOLO-Model-Label-Changer
   ```

3. Open the `yolo_changer.ipynb` Jupyter Notebook.

4. Update the file path for the pre-trained YOLO model in the following line:

   ```python
   model = YOLO("model_car_parts.pt")
   ```

5. In the "Change Labels" section, update the `car_parts_class_mapping` dictionary with the new class names you want to use:

   ```python
   car_parts_class_mapping = {
       0: 'Alloy-Rim_BLS',
       1: 'Alloy-Rim_BRS',
       2: 'Alloy-Rim_FLS',
       3: 'Alloy-Rim_FRS',
       4: 'Antenna',
       5: 'Back-Bumper',
       6: 'Back-Logo',
   }
   ```

6. Run the cells in the notebook to update the model's class names and save the updated model.

7. The updated model will be saved to a new file named `model_updated.pt`.

## Requirements

- Python 3.x
- Jupyter Notebook
- Ultralytics YOLO library (`pip install ultralytics`)

## Acknowledgements

This project was inspired by the need to update class names in a pre-trained YOLO model for a specific use case. The script provides a simple and efficient way to accomplish this task.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
