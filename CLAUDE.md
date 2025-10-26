# OHLC Model - Project Memory

## Project Structure

**Code folder:** `D:\Programming\ohlc_model` - Contains model code, notebooks, and configuration
**Data folder:** `D:\Programming\ohlc_model\raw_data` - Raw input datasets
**Processed Data:** `D:\Programming\ohlc_model\preprocessed_data` - Cleaned and normalized datasets

## Project Context - TCN Deep Learning Model

**Project Type:** OHLC Time Series Forecasting using Temporal Convolutional Networks
**Focus Areas:** 
- OHLC (Open, High, Low, Close) stock price forecasting
- Nifty 50 index prediction
- Deep learning model development and evaluation

## Key Files

- **Main Model:** `code/TCN_deep_learning_model.ipynb` - Primary TCN implementation
- **Data Source:** `nifty_50_historical_data.csv` - Historical OHLC data
- **Trained Model:** `tcn_nifty_model.h5` - Saved model weights
- **Documentation:** `README.md` - Project overview and setup

## Development Standards

### Code Quality
- Use clean, efficient Python code
- Follow PEP 8 style guidelines
- Include docstrings and comments for complex logic
- Optimize model training for minimal computational overhead

### Model Development
- Focus on TCN architecture efficiency
- Proper data normalization and preprocessing
- Train/validation/test split discipline
- Model evaluation with appropriate metrics (MAE, MSE, RMSE)

### Data Management
- Keep raw and processed data separate
- Document data preprocessing steps
- Version control notebook changes only (not data files due to .gitignore)
- Handle missing values appropriately

## Git Workflow

### Automated Git Management
- All code changes are automatically staged, committed, and pushed
- Commit format: `[#N]: Brief message` (max 10 words)
- Auto-triggers: New features, bug fixes, model updates, "Update project" command

### Repository Details
- **Repository:** `ohlc_model`
- **Owner:** `ShashwatGold1`
- **Branch:** `main`
- **Remote:** `https://github.com/ShashwatGold1/ohlc_model.git`

## File Management Rules

- Only create files when absolutely necessary
- Prefer editing existing files over creating new ones
- Never proactively create documentation unless explicitly requested
- Maintain proper `.gitignore` configuration

## Model Architecture Notes

**TCN (Temporal Convolutional Network):**
- Uses dilated convolutions for capturing long-range dependencies
- Effective for time series forecasting tasks
- Input: OHLC features with lookback window
- Output: Price predictions (next period OHLC or close price)

## Large File Analysis Protocol

For files exceeding context limits:
1. Use grep_search tool with pattern matching
2. Never use read_file for large datasets (CSV, etc.)
3. Apply strategic filtering to locate relevant data
4. Extract precise matches with line numbers

## Recent Changes

- Initial project setup and Git initialization
- Created `.gitignore` for Python environments and data files
- Added comprehensive `README.md`
- First commit: "Initial commit: TCN deep learning model for OHLC forecasting"

## Next Steps

- Push repository to GitHub (requires GitHub auth)
- Develop TCN model training pipeline
- Implement data preprocessing for OHLC features
- Create model evaluation metrics and visualization
- Deploy trained model for inference
