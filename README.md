## Comparing Prompting Techniques Through Engineering Problem-Solving Scenarios
NAME:R.DHIVYA

### AIM

To compare different prompting techniques and evaluate their effectiveness in solving a real-world engineering problem using an AI system.

### AI TOOLS REQUIRED

* ChatGPT


### PROJECT TITLE

**AI-Based Crop Disease Detection Using Computer Vision**

### PROBLEM STATEMENT

Farmers often find it difficult to identify crop diseases at an early stage. Manual identification requires expert knowledge and may take more time. The proposed system uses computer vision and artificial intelligence to detect crop diseases from leaf images and provide the disease name with suitable recommendations.

### SELECTED ENGINEERING SCENARIO

The selected scenario is **detecting crop diseases from leaf images using AI and computer vision**.

---

## PROCEDURE

### Step 1 – Select the Engineering Problem

A genuine problem from the project is selected. In this experiment, the problem is detecting crop diseases from leaf images.

### Step 2 – Write the Base Prompt

A simple prompt is created without giving detailed instructions.

**Base Prompt:**

Suggest a method to detect crop diseases using computer vision.

### Step 3 – Apply Different Prompting Techniques

### Technique 1 – Straightforward Prompt

Suggest a method to detect crop diseases using computer vision.

### Technique 2 – Role-Based Prompt

Act as an AI engineer. Suggest an effective computer vision method for detecting crop diseases from leaf images. Mention the suitable model and basic working steps.

### Technique 3 – Few-Shot Prompt

Example 1: Input – Healthy tomato leaf → Output – Healthy.
Example 2: Input – Tomato leaf with yellow spots → Output – Possible leaf disease.
Now suggest a computer vision method that can classify crop diseases from leaf images.

### Technique 4 – Step-by-Step Prompt

Explain step-by-step how to develop a crop disease detection system using computer vision. Include image collection, preprocessing, model training, testing and prediction.

### Technique 5 – Constraint-Based Prompt

Design a crop disease detection system using computer vision. Use a CNN-based model, explain the preprocessing and training steps, and suggest suitable evaluation metrics. Keep the solution practical for a student project.

---

# AI-GENERATED OUTPUTS

### Output for Straightforward Prompt

## **Method: CNN-Based Crop Disease Detection Using Computer Vision**

A practical method for detecting crop diseases is to use a **Convolutional Neural Network (CNN)** to classify images of crop leaves as healthy or diseased.

### **Working procedure**

1. **Image collection:** Collect labelled images of healthy and diseased crop leaves using a camera or a public dataset such as PlantVillage.
2. **Image preprocessing:** Resize images to 224 × 224 pixels, normalize pixel values, and remove unnecessary noise.
3. **Data augmentation:** Apply rotation, flipping, zooming, and brightness changes to improve model generalization.
4. **Model selection:** Use a CNN model such as MobileNetV3 or ResNet50. MobileNetV3 is suitable for student projects because it is lightweight and can be deployed on mobile devices.
5. **Model training:** Train the model using labelled leaf images and validate its performance on separate images.
6. **Disease prediction:** Provide a new leaf image to the trained model. The model predicts the disease class and generates a confidence score.
7. **Performance evaluation:** Evaluate the model using accuracy, precision, recall, F1-score, and a confusion matrix.

### **System architecture**

Crop leaf image

Image preprocessing and augmentation

CNN / MobileNetV3 model

Disease classification

Disease name and confidence score

### **Expected output**

For example, when a tomato leaf image is provided, the system may produce:

- Crop: Tomato
- Predicted disease: Early blight
- Confidence score: 94.5%

The confidence score represents the model's prediction, not a guarantee of disease diagnosis.

### **Recommended tools**

| Component               | Tool                                     |
| ----------------------- | ---------------------------------------- |
| Programming language    | Python                                   |
| Deep learning framework | TensorFlow / Keras                       |
| Image processing        | OpenCV                                   |
| Dataset                 | PlantVillage                             |
| Model                   | MobileNetV3                              |
| Deployment              | Flask web application or TensorFlow Lite |

**Conclusion:** A CNN-based image classification system using MobileNetV3 transfer learning is a practical and effective starting point for a student engineering project on AI-based crop disease detection. It can identify disease categories from leaf images and can be extended to estimate disease severity or provide treatment recommendations.

### Output for Role-Based Prompt

## **AI-Based Crop Disease Detection Using Computer Vision**

As an AI engineer, I recommend using a **CNN-based image classification system with MobileNetV3 transfer learning** to detect crop diseases from leaf images.

### **1. Suitable model**

**MobileNetV3** is a lightweight deep learning model suitable for crop disease classification. It can identify healthy and diseased leaves and distinguish between different disease categories.

It is particularly suitable for student engineering projects because it requires less computational power than many larger CNN models and can be deployed on mobile devices.

### **2. Basic working steps**

1. **Image collection:** Collect labelled images of healthy and diseased crop leaves using a camera or a public dataset such as PlantVillage.
2. **Image preprocessing:** Resize images to 224 × 224 pixels and normalize pixel values.
3. **Data augmentation:** Apply rotation, flipping, zooming, and brightness adjustments to improve model generalization.
4. **Model training:** Use a pretrained MobileNetV3 model and fine-tune it with the collected leaf images.
5. **Disease classification:** The trained model analyzes the input image and predicts the corresponding disease class.
6. **Model evaluation:** Test the model using unseen images and calculate accuracy, precision, recall, F1-score, and a confusion matrix.
7. **Prediction:** Display the predicted disease name and confidence score to the user.

### **3. System workflow**

Crop leaf image

Image preprocessing and augmentation

MobileNetV3 CNN model

Disease classification

Disease name and confidence score

### **4. Expected output**

For example, when a tomato leaf image is provided:

- Crop: Tomato
- Predicted disease: Early blight
- Confidence score: 94.5%

The confidence score indicates the model's prediction confidence and does not guarantee a correct diagnosis.

### **Conclusion**

A CNN-based crop disease detection system using MobileNetV3 transfer learning is an effective and practical approach. It can classify crop leaf images into healthy and diseased categories and identify specific diseases. The system can be further improved by incorporating disease severity estimation and a mobile application for farmers.

### Output for Few-Shot Prompt

## **Computer Vision Method for Crop Disease Classification**

A suitable method is to use a **Convolutional Neural Network (CNN) with transfer learning**, such as MobileNetV3, to classify crop leaf images into healthy and diseased categories.

### **Basic working steps**

1. **Image collection:** Collect labelled images of healthy and diseased crop leaves, such as tomato leaves affected by early blight, late blight, or leaf mold.
2. **Image preprocessing:** Resize images to 224 × 224 pixels and normalize pixel values.
3. **Model training:** Train a CNN model using the labelled images. Transfer learning with MobileNetV3 can improve performance while reducing training time.
4. **Image classification:** Provide a new leaf image to the trained model. The model extracts visual features such as spots, discoloration, and lesions to predict the disease category.
5. **Output generation:** Display the predicted disease name and confidence score.
6. **Performance evaluation:** Evaluate the model using accuracy, precision, recall, and F1-score.

### **Example**

| Input image                             | Predicted output                                   |
| --------------------------------------- | -------------------------------------------------- |
| Healthy tomato leaf                     | Healthy                                            |
| Tomato leaf with yellow spots           | Possible disease                                   |
| Tomato leaf with brown circular lesions | Early blight (if supported by the trained classes) |

### **Conclusion**

A CNN-based classification system using MobileNetV3 is a practical solution for crop disease detection. It can automatically classify leaf images and identify possible diseases, helping farmers recognize crop health problems at an early stage. The model should be trained on representative images of each disease to ensure reliable predictions.

### Output for Step-by-Step Prompt

## **Step-by-Step Development of a Crop Disease Detection System Using Computer Vision**

A crop disease detection system can be developed using **Convolutional Neural Networks (CNNs)** to analyze leaf images and identify whether a plant is healthy or affected by a particular disease.

The following steps describe the complete development process.

### **Step 1: Image Collection**

- Collect images of healthy and diseased crop leaves using a smartphone or digital camera.
- Use publicly available datasets such as PlantVillage.
- Organize images into categories based on crop type and disease name.
- Ensure that each image has the correct disease label.

### **Step 2: Image Preprocessing**

- Resize all images to a standard size, such as 224 × 224 pixels.
- Normalize pixel values to improve model training.
- Remove unnecessary noise and unwanted background information where appropriate.
- Convert images into a suitable format for the deep learning model.

### **Step 3: Data Augmentation**

Apply image transformations to increase dataset diversity.

Examples:

- Rotation
- Horizontal flipping
- Zooming
- Brightness adjustment
- Image shifting

This helps the model generalize better to new images.

### **Step 4: Dataset Splitting**

Divide the collected dataset into three groups:

- Training dataset: 70% of images.
- Validation dataset: 15% of images.
- Testing dataset: 15% of images.

The training dataset is used to train the model, the validation dataset helps tune it, and the testing dataset evaluates its final performance. Keep images from the same plant or capture session in only one split to avoid data leakage.

### **Step 5: Model Selection and Training**

- Select a suitable CNN architecture such as MobileNetV3, ResNet50, or EfficientNet.
- Use MobileNetV3 for a lightweight student project.
- Train the model using the labelled leaf images.
- Adjust parameters such as learning rate, batch size, and number of epochs.
- Fine-tune the pretrained model to improve classification performance.

### **Step 6: Model Testing**

- Provide unseen leaf images to the trained model.
- Compare predicted disease labels with actual labels.
- Calculate performance metrics such as:
  - Accuracy
  - Precision
  - Recall
  - F1-score
- Use a confusion matrix to identify classification errors.

### **Step 7: Disease Prediction**

- Capture or upload a new crop leaf image.
- Apply the same preprocessing techniques used during training.
- Pass the image to the trained CNN model.
- Predict the disease category based on the model's output probabilities.
- Display the disease name and confidence score.

### **Step 8: Application Development**

- Integrate the trained model into a simple web or mobile application.
- Allow farmers to upload or capture leaf images.
- Display the predicted disease and suitable agricultural recommendations.
- Use TensorFlow Lite for mobile deployment or Flask for web deployment.

For example, when a tomato leaf image is uploaded:

**Input: Healthy tomato leaf**

Healthy

**Input: Diseased tomato leaf**

Early blight


### **Conclusion**

A crop disease detection system can be developed using computer vision and CNN-based deep learning models. By following image collection, preprocessing, augmentation, model training, testing, and prediction steps, the system can automatically identify crop diseases from leaf images. This approach can help farmers detect diseases early and take appropriate preventive measures.

### Output for Constraint-Based Prompt
## **AI-Based Crop Disease Detection Using Computer Vision**

**Proposed method:** Use a Convolutional Neural Network (CNN) with MobileNetV3 to identify crop diseases from leaf images.

### **1. Image Collection**

- Collect healthy and diseased leaf images.
- Use the PlantVillage dataset.
- Label images according to disease categories.

### **2. Image Preprocessing**

- Resize images to 224 × 224 pixels.
- Normalize pixel values.
- Apply rotation, flipping and zooming to increase image variety.

### **3. Model Selection**

Use **MobileNetV3**, a lightweight CNN model suitable for image classification and mobile applications.

### **4. Model Training**

- Split the dataset into 70% training, 15% validation and 15% testing.
- Train the CNN using labelled images.
- Use transfer learning to improve performance.

### **5. Disease Prediction**

Upload a new leaf image to the trained model. The model predicts whether the leaf is healthy or diseased and displays the disease name.

### **6. Evaluation Metrics**

Evaluate the model using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

### **7. Tools Required**

| Component        | Technology   |
| ---------------- | ------------ |
| Programming      | Python       |
| Deep learning    | TensorFlow   |
| Image processing | OpenCV       |
| Dataset          | PlantVillage |
| Model            | MobileNetV3  |
| Interface        | Flask        |

### **Expected Output**

- Input: Tomato leaf image.
- Output: Early blight detected.
- Confidence: 94.5% (illustrative).

### **Conclusion**

A CNN-based crop disease detection system using MobileNetV3 provides a practical solution for identifying crop diseases from leaf images. It is affordable, easy to implement and suitable for a student engineering project.

---

# COMPARISON / EVALUATION TABLE

| Prompting Technique | Relevance | Accuracy  | Completeness | Clarity   | Feasibility | Usefulness |
| ------------------- | --------- | --------- | ------------ | --------- | ----------- | ---------- |
| Straightforward     | Good      | Good      | Moderate     | Good      | Good        | Moderate   |
| Role-Based          | Very Good | Very Good | Good         | Very Good | Very Good   | Very Good  |
| Few-Shot            | Good      | Good      | Moderate     | Good      | Good        | Good       |
| Step-by-Step        | Very Good | Very Good | Very Good    | Very Good | Very Good   | Very Good  |
| Constraint-Based    | Excellent | Very Good | Excellent    | Very Good | Excellent   | Excellent  |

---

# ANALYSIS AND OBSERVATIONS

The experiment shows that the quality of the AI response depends strongly on how the prompt is written. The straightforward prompt provides a general solution but does not contain enough details.

The role-based prompt gives a more professional response because the AI is given a specific role. The few-shot prompt helps the AI understand the expected type of output through examples.

The step-by-step prompt produces a well-organized solution and covers the complete development process. The constraint-based prompt gives the most practical response because it specifies the model type, evaluation metrics and project requirements.

Overall, **clear and structured prompts provide better quality, accuracy and depth than simple prompts**. However, naïve prompts can still be useful when only a quick general idea is required.

---

# FINAL SELECTED PROMPTING TECHNIQUE

**Constraint-Based Prompting** was selected as the most suitable technique because it provides a detailed, practical and project-oriented response while controlling the expected output.

### REFINED / FINAL PROMPT

> Act as an AI and computer vision engineer. Design a practical crop disease detection system using leaf images. Use a CNN or transfer-learning model. Explain the complete workflow including dataset collection, image preprocessing, data augmentation, model training, validation, testing and disease prediction. Suggest suitable evaluation metrics such as accuracy, precision, recall and F1-score. Keep the solution simple enough for a student engineering project and mention possible limitations and improvements.

---

# ENGINEERING VALIDATION

The suggested approach is technically feasible for an engineering project because crop leaf images can be collected and classified using CNN or transfer-learning models. The system can be tested using a separate test dataset and evaluated using standard classification metrics such as accuracy, precision, recall and F1-score.

The final model can be integrated into a simple web or mobile application where the user uploads a crop leaf image and receives the predicted disease class.

---

# CONCLUSION

Different prompting techniques were tested for the crop disease detection problem. Constraint-based prompting provided the most practical and detailed solution. Structured prompts generally produced better results than simple prompts.

### RESULT

Different prompting techniques were successfully compared, and Constraint-Based Prompting was identified as the most effective technique for the selected engineering problem.
