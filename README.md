# Airbnb Price Predictor

## Overview
This project predicts Airbnb listing prices using machine learning techniques like XGBoost and Neural Networks

## Installation

```bash
git clone <repository-url>
cd Airbnb-price-predictor
pip install -r requirements.txt
```
## Download the Data 
Download the provided data.zip file from this repository or the course source. Unzip the Data and Extract the contents of data.zip.
 

## Data Table

<table>
  <thead>
    <tr>
      <th>City Market</th>
      <th>Density Tier</th>
      <th>Data Month</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>New York City, NY</strong></td>
      <td>Tier 1: Big</td>
      <td>Oct 2025</td>
    </tr>
    <tr>
      <td><strong>Los Angeles, CA</strong></td>
      <td>Tier 1: Big</td>
      <td>Sep 2025</td>
    </tr>
    <tr>
      <td><strong>San Francisco, CA</strong></td>
      <td>Tier 1: Big</td>
      <td>sep 2025</td>
    </tr>
    <tr>
      <td><strong>Chicago, IL</strong></td>
      <td>Tier 1: Big</td>
      <td>June 2025</td>
    </tr>
    <tr>
      <td><strong>Austin, TX</strong></td>
      <td>Tier 2: Medium</td>
      <td>June 2025</td>
    </tr>
    <tr>
      <td><strong>Seattle, WA</strong></td>
      <td>Tier 2: Medium</td>
      <td>September 2025</td>
    </tr>
    <tr>
      <td><strong>Denver, CO</strong></td>
      <td>Tier 2: Medium</td>
      <td>sep 2025</td>
    </tr>
    <tr>
      <td><strong>Portland, OR</strong></td>
      <td>Tier 2: Medium</td>
      <td>Sept 2025</td>
    </tr>
    <tr>
      <td><strong>Asheville, NC</strong></td>
      <td>Tier 3: Small</td>
      <td>June 2025</td>
    </tr>
    <tr>
      <td><strong>Santa Cruz, CA</strong></td>
      <td>Tier 3: Small</td>
      <td>June 2025</td>
    </tr>
    <tr>
      <td><strong>Salem, OR</strong></td>
      <td>Tier 3: Small</td>
      <td>Sep 2025</td>
    </tr>
    <tr>
      <td><strong>Columbus, OH</strong></td>
      <td>Tier 3: Small</td>
      <td>Sept 2025</td>
    </tr>
  </tbody>
</table>

<section>
  <h2>Major Findings: XGBoost vs. Neural Networks</h2>

  <h3>Tier-Based Performance</h3>
  <ul>
    <li><strong>XGBoost</strong>  provided higher stability due to its handling of tabular outliers in complex markets.</li>
    <li><strong>Best Model:</strong> XGBoost generally won in terms of R2 Score and MAE across most individual cities.</li>
  </ul>

  <h3>Market Generalization</h3>
  <ul>
    <li> Tier 1 models successfully identified high-level drivers that remained constant across city sizes as the dataset size was way larger compared to medium and small cities </li>
    <li>Generalization dropped when small cities models predicted big cities  prices, proving market stratification matters.</li>
  </ul>

  <h3>Conclusion</h3>
  <p><em>XGBoost remains the tabular benchmark, but Neural Networks are effective for generalization.</em></p>
</section>
