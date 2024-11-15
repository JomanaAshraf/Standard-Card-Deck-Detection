# **Standard 52-Cards Deck Object Detection**

This project focuses on detecting the standard 52-card deck, with each card represented as a unique class. The object detection task was accomplished using the **YOLOv7 architecture**, a state-of-the-art model for object detection known for its speed and accuracy.

---

## **Project Description**
The objective of this project is to identify individual cards from a standard 52-card deck. Each card is treated as a separate class, with class names based on the card value and suit.

### **Classes**
The 52 classes represent all cards in a standard deck. The naming convention is as follows:
- **Value**: Numbers (2-10), Ace (A), Jack (J), Queen (Q), and King (K).
- **Suit**: 
  - **S**: Spades
  - **C**: Clubs
  - **D**: Diamonds
  - **H**: Hearts

Example class names:
`['10C', '10D', '10H', '10S', '2C', '2D', '2H', '2S', ..., 'QC', 'QD', 'QH', 'QS']`

---

## **Methodology**
1. **Dataset Preparation**:
   - The dataset was created and labeled using [Roboflow](https://roboflow.com/), an efficient tool for image annotation and dataset preparation.
   - [Link to the Roboflow Dataset](https://app.roboflow.com/test-9yul0/cards_dataset/1)

2. **Model Architecture**:
   - The YOLOv7 object detection framework was employed for its cutting-edge accuracy and real-time performance capabilities.

3. **Training Process**:
   - Images were pre-processed and annotated using Roboflow.
   - YOLOv7 was trained with labeled data to detect and classify all 52 card types accurately.

---

## **Results**
- The trained YOLOv7 model achieves high accuracy in detecting and classifying all 52 card types.
- Outputs include bounding boxes around detected cards, labeled with their corresponding class.
