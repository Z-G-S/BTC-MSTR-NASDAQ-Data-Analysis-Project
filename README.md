# BTC-MSTR-NASDAQ-Data-Analysis-Project
Contains a data analysis project in Excel and SPSS that explores the relationship between the price growth of Bitcoin and the price growth of MicroStrategy.

# Summary
_A detailed report on the data analysis project can be found in the **DataAnalysisProject_Report.pdf** section, this section will contain a brief introduction, objectives of the model, some of the pre-processing steps and the output._

**Introduction & Rationale**

The model explores the relationship between the price growth of Bitcoin (BTC) and the price growth of MicroStrategy (MSTR) from 11/08/2020 to 09/12/2023, with some references to NASDAQ. MicroStrategy owns such a significant holding of Bitcoin, so much so that every 1 in 120 Bitcoin's are owned by MicroStrategy. Therefore the rationale behind the model is to explore whether the price growth of Bitcoin impacts the price growth of MSTR, due to their large holding of Bitcoin. The analysis of outputs in the report provide stakeholders such as shareholders or other investors with insightful information and visualisations that they can use to enhance financial decision making.

**Objectives**

1. Determine the strength of the relationship between the price growth of BTC and the price growth of MSTR.
   Measured using Pearson’s Correlation Coefficient (r), and the Coefficient of Determination (r2) to determine how well the statistical model explains the variance of the dependent variable (MSTR). 
   Visualised using a Line Graph and Scatter Plot.
3. Compare the daily volatility of MSTR to NASDAQ.
   Measured using summary statistics such as mean and standard deviation.
   Visualised using Histograms, Normal Q-Q Plots and Detrended Normal Q-Q Plots.
4. Draw empirical conclusions to provide stakeholders with useful insights for decision-making.

**Overview of processing steps**

_Excel_: Using the MATCH function to align dates

BTC is open for trade everyday whereas MSTR and NASDAQ is only open for trade on non-holiday weekdays. This caused a misalignment in the date variable column. To fix this, the MATCH function was used to search the BTC date values in the MSTR?NASDAQ date values, returning #N/A if missing. From here, the missing dates were pasted at the end of the MSTR/NASDAQ date variable column, sorted from oldest to newest which aligned values, and the duplicate date variable was subsequently deleted. The series of images below show the origional dataset (note the misalignment with the date variable values) and the processed dataset with aligned dates and a pattern of missing values for MSTR and NASDAQ associated variables.

![Screenshot 2024-02-10 005526](https://github.com/Z-G-S/BTC-MSTR-NASDAQ-Data-Analysis-Project/assets/140622522/4b8b4d94-7c8b-4d27-8fb1-7b97f232528f)
![Screenshot 2024-02-10 005538](https://github.com/Z-G-S/BTC-MSTR-NASDAQ-Data-Analysis-Project/assets/140622522/4078cee7-21ae-4b6b-89d7-17e5533f433a)

_SPSS_: Dealing with missing values

The missing values in the MSTR and NASDAQ variables were dealt in the Missing Values Handler in SPSS. The method used was 'Mean of nearby points' with a span of two.

**Output**

![Screenshot 2024-02-10 005942](https://github.com/Z-G-S/BTC-MSTR-NASDAQ-Data-Analysis-Project/assets/140622522/4e32ee76-2284-456a-9b51-055e49befb1e)
![Screenshot 2024-02-10 005932](https://github.com/Z-G-S/BTC-MSTR-NASDAQ-Data-Analysis-Project/assets/140622522/764ba578-5f8a-4392-962a-49d6d7268fb9)
![Screenshot 2024-02-10 005921](https://github.com/Z-G-S/BTC-MSTR-NASDAQ-Data-Analysis-Project/assets/140622522/7ad9274a-4e56-46b0-8a13-48aeca5479c4)
![Screenshot 2024-02-10 005910](https://github.com/Z-G-S/BTC-MSTR-NASDAQ-Data-Analysis-Project/assets/140622522/2bf9e5b4-d1de-456d-a757-32d13e62607f)
![Screenshot 2024-02-10 005858](https://github.com/Z-G-S/BTC-MSTR-NASDAQ-Data-Analysis-Project/assets/140622522/2ab1c060-24da-4d65-a0c4-c5fdaa942f90)
