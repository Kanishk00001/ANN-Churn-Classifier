# Customer Churn Prediction with Neural Networks

Predicting which customers might leave before they actually do. Built this to help businesses keep their customers happy and reduce churn rates.

**[Check out the live app here](https://ann-churn-classifier-a3wvkhpe5pvezsmwpzaqmf.streamlit.app/)**

## What's this about?

Customer churn is expensive. When customers leave, businesses lose revenue and have to spend more money finding new ones. This project uses machine learning to spot patterns in customer behavior that might indicate they're thinking about leaving.

The idea is simple - if you can predict who's about to leave, you can try to keep them around with better offers, customer service, or other retention strategies.

## How it works

I built a neural network that looks at customer data like:
- How long they've been with the company
- Their monthly spending
- What services they use
- Payment methods and contract types
- Demographics like age and location

The model learns from historical data of customers who stayed vs. those who left, then makes predictions on new customers.

## What you can do with it

The Streamlit app lets you:
- Input customer information and get churn predictions
- See which factors are most important for the prediction
- Upload your own customer data for batch predictions
- Visualize the model's performance and decision boundaries

## Running it yourself

**Get the code:**
```bash
git clone https://github.com/Kanishk00001/ANN-Churn-Classifier.git
cd ANN-Churn-Classifier
```

**Install what you need:**
```bash
pip install -r requirements.txt
```

**Run the app:**
```bash
streamlit run app.py
```

## The technical stuff

Built with:
- **TensorFlow/Keras** for the neural network
- **Streamlit** for the web interface
- **Pandas** and **NumPy** for data handling
- **Scikit-learn** for preprocessing and metrics
- **Matplotlib/Seaborn** for visualizations

The neural network architecture is pretty straightforward:
- Input layer with customer features
- A few hidden layers with dropout for regularization
- Output layer with sigmoid activation for binary classification

## Files and folders

```
├── app.py              # Main Streamlit application
├── model.py            # Model training and prediction logic
├── data/               # Dataset files
├── models/             # Saved model files
├── notebooks/          # Jupyter notebooks for experiments
└── requirements.txt    # Python dependencies
```

## Results

The model performs reasonably well on the test data. You can see detailed metrics and confusion matrices in the Streamlit app.

Some interesting findings:
- Contract type and tenure are strong predictors
- Monthly charges matter more than total charges
- Customers with electronic check payments churn more often

## Next steps

Things I'd like to add:
- More advanced feature engineering
- Different model architectures (maybe try XGBoost)
- Real-time model retraining capabilities
- Integration with business intelligence tools

## Contributing

Found a bug or have an idea? Feel free to open an issue or submit a pull request. Always happy to collaborate!

---

Built by [Kanishk](https://github.com/Kanishk00001)
