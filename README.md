<div align="center">

  <h1>📸 Instagram Reach & Audience Engagement Analytics</h1>
  <p><b>Advanced Exploratory Data Analysis (EDA) on Post Reach Channels, Follower Funnels, and Content Dynamics</b></p>

  <p>
    <img src="https://img.shields.io/badge/Python-3.9%2B-3776AB?style=for-the-badge&logo=python&logoColor=white" />
    <img src="https://img.shields.io/badge/Pandas-Data%20Engineering-150458?style=for-the-badge&logo=pandas&logoColor=white" />
    <img src="https://img.shields.io/badge/Seaborn-Statistical%20Plots-4c72b0?style=for-the-badge" />
    <img src="https://img.shields.io/badge/Matplotlib-Visualization-11557c?style=for-the-badge" />
    <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" />
  </p>

</div>

<hr />

<h2>📌 Executive Summary & Core Insights</h2>
<p>
This project conducts an exhaustive evaluation of Instagram post performance metrics. By analyzing real post data, we isolate the fundamental drivers behind content reach, user retention, and organic conversion funnels:
</p>

<ul>
  <li><b>Impression Origin Dominance:</b> The <b>Home Feed (~42.9%)</b> and <b>Hashtags (~33.8%)</b> form the backbone of organic discovery, accounting for over <b>76.7%</b> of cumulative audience exposure.</li>
  <li><b>The Conversion Funnel:</b> Statistical correlation proves that <b>Shares &rarr; Profile Visits &rarr; Follows</b>. Direct peer shares represent the most leveraged channel for turning passive scrollers into long-term subscribers.</li>
  <li><b>Quality Signals:</b> Total impressions scale with high positive elasticity against <b>Saves</b> and <b>Comments</b>, verifying that educational and reference-grade content extends distribution longevity.</li>
  <li><b>Copy Length Impact:</b> Contrary to the assumption that short copy is always best, detailed, descriptive captions correlate positively with increased like volume.</li>
</ul>

<hr />

<h2>🛠️ Analytical Pipeline & Architecture</h2>

<table width="100%">
  <tr>
    <td width="33%" align="center"><b>1. ETL & Preprocessing</b></td>
    <td width="33%" align="center"><b>2. Feature Engineering</b></td>
    <td width="33%" align="center"><b>3. Statistical Modeling</b></td>
  </tr>
  <tr>
    <td>
      • Ingestion using Latin-1 encoding<br />
      • Deduplication (purged 17 duplicates)<br />
      • Null auditing across 13 native metrics
    </td>
    <td>
      • <code>Caption_Words</code> (word count tokenization)<br />
      • <code>Hashtags_count</code> (tag frequency)<br />
      • <code>Total_Engagement</code> (Likes + Comments + Follows)<br />
      • <code>top_way</code> (dominant reach route)
    </td>
    <td>
      • Multi-channel contribution analysis<br />
      • Linear regression plots via Seaborn<br />
      • Conversion rate funnel mapping
    </td>
  </tr>
</table>

<hr />

<h2>🔬 Data Ingestion & Transformation</h2>

<table width="100%">
  <tr>
    <th width="50%" align="center">Raw Data Structure</th>
    <th width="50%" align="center">Verified Cleaned Dataset</th>
  </tr>
  <tr>
    <td align="center">
      <img src="https://i.postimg.cc/RVLYd31p/shkl-aldata.png" alt="Raw Data Structure" width="100%" />
      <p><i>Raw dataset schema containing 119 records before cleaning.</i></p>
    </td>
    <td align="center">
      <img src="https://i.postimg.cc/pXJSC9Qs/bʿd-alklynynj.png" alt="Cleaned Matrix" width="100%" />
      <p><i>102 verified transactional instances after removing redundancy.</i></p>
    </td>
  </tr>
</table>

<h3>Feature Engineering Matrix</h3>
<div align="center">
  <img src="https://i.postimg.cc/SNfPdXLD/bʿd-aladafh.png" alt="Feature Engineering Matrix" width="95%" />
  <p><i>Synthesized attributes: Caption_Words, Hashtags_count, and Primary Traffic Routes.</i></p>
</div>

<hr />

<h2>📊 Statistical Visualizations & Business Intelligence</h2>

<h3>1. Traffic Origin & Reach Distribution</h3>
<p>
Comparing traffic channels highlights that the <b>Home Feed</b> secures baseline visibility with active followers, while <b>Hashtags</b> and <b>Explore</b> provide organic external exposure.
</p>

<table width="100%">
  <tr>
    <th width="50%" align="center">Traffic Route Contribution</th>
    <th width="50%" align="center">Total Impressions by Channel</th>
  </tr>
  <tr>
    <td align="center">
      <img src="https://i.postimg.cc/gkH7swyH/bay-shart.png" alt="Impression Distribution Pie" width="95%" />
    </td>
    <td align="center">
      <img src="https://i.postimg.cc/ZKxQH9PP/bar-shart.png" alt="Channel Bar Chart" width="95%" />
    </td>
  </tr>
  <tr>
    <td colspan="2">
      <b>Business Takeaway:</b> Home and Hashtags account for over 3/4 of overall visibility. Strategic hashtag curation is essential for expanding reach beyond existing followers.
    </td>
  </tr>
</table>

<br />

<h3>2. Content Longevity & Algorithm Triggers</h3>

<table width="100%">
  <tr>
    <th width="50%" align="center">Saves vs. Total Impressions</th>
    <th width="50%" align="center">Likes vs. Total Impressions</th>
  </tr>
  <tr>
    <td align="center">
      <img src="https://i.postimg.cc/L6p7jkPD/alhfz-balambryshnz.png" alt="Saves vs Impressions" width="95%" />
    </td>
    <td align="center">
      <img src="https://i.postimg.cc/pLV662qM/layks-balambryshnz.png" alt="Likes vs Impressions" width="95%" />
    </td>
  </tr>
  <tr>
    <td colspan="2">
      <b>Business Takeaway:</b> High save rates show a clear upward trend with total reach. Educational, reference-style posts provide sustained utility that keeps the post circulating longer.
    </td>
  </tr>
</table>

<br />

<h3>3. Explore Placement Dynamics</h3>
<div align="center">
  <img src="https://i.postimg.cc/pXJSC9Qw/ʿlaqt-alaksblw-ballayks.png" alt="Explore vs Likes" width="75%" />
  <p><b>Business Takeaway:</b> Positive regression slope proving that posts clearing early follower interaction thresholds are favored for organic Explore page placement.</p>
</div>

<br />

<h3>4. The Follower Acquisition Funnel</h3>

<table width="100%">
  <tr>
    <th width="50%" align="center">Shares vs. Profile Visits</th>
    <th width="50%" align="center">Profile Visits vs. New Follows</th>
  </tr>
  <tr>
    <td align="center">
      <img src="https://i.postimg.cc/dtjf67mK/ʿlaqt-alshyr-b-zyart-alakwnt.png" alt="Shares vs Profile Visits" width="95%" />
    </td>
    <td align="center">
      <img src="https://i.postimg.cc/YC2ssp8P/ʿlaqt-alfwlwz-b-zyart-alakwnt.png" alt="Visits vs Follows" width="95%" />
    </td>
  </tr>
  <tr>
    <td colspan="2">
      <b>Business Takeaway:</b> Shares generate the strongest conversion into profile visits, and those visits convert directly into new followers. Optimizing for shareability is key to account growth.
    </td>
  </tr>
</table>

<br />

<h3>5. Copy Dynamics: Caption Word Count vs. Engagement</h3>
<div align="center">
  <img src="https://i.postimg.cc/mgZ55bV0/ʿlaqt-alkabshn-b-allayks.png" alt="Caption Length vs Likes" width="75%" />
  <p><b>Business Takeaway:</b> Descriptive, well-structured captions lead to longer dwell times and higher likes, debunking the belief that ultra-short copy is always best.</p>
</div>

<hr />

<h2>🏆 Top-Performing Content Benchmark</h2>

<div align="center">
  <img src="https://i.postimg.cc/qMxFwtcm/twb-bwst.png" alt="Top Performing Post" width="90%" />
</div>

<table width="100%">
  <tr>
    <th align="center">Total Engagement</th>
    <th align="center">Likes</th>
    <th align="center">Comments</th>
    <th align="center">Follows Generated</th>
    <th align="center">Primary Route</th>
  </tr>
  <tr>
    <td align="center"><b>765 Actions</b></td>
    <td align="center">549</td>
    <td align="center">2</td>
    <td align="center">214</td>
    <td align="center">Home / Explore</td>
  </tr>
</table>

<p>
<i>Content centered around actionable career paths and technical certification guides yielded the highest engagement and follower conversion across the entire dataset.</i>
</p>

<hr />

<h2>🚀 Installation & Quickstart</h2>

<pre><code># 1. Clone repository
git clone https://github.com/Abdallah-Elsayed-1/instagram-account-analytics.git
cd instagram-account-analytics

# 2. Set up virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# 3. Install analytical dependencies
pip install pandas numpy matplotlib seaborn jupyter

# 4. Launch Jupyter Notebook
jupyter notebook "Analysis for instagram account.ipynb"</code></pre>

<hr />

<h2>👨‍💻 Author & Contact</h2>

<p>
<b>Abdallah Elsayed</b><br />
<i>Data Analyst & Business Intelligence Specialist</i>
</p>

<p>
  <a href="https://www.linkedin.com/in/abdallah-elsayed-d1" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-Profile-blue?style=flat&logo=linkedin" />
  </a>
  <a href="https://github.com/Abdallah-Elsayed-1" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-Portfolio-darkgreen?style=flat&logo=github" />
  </a>
  <a href="mailto:abdallahhelsayedd@gmail.com">
    <img src="https://img.shields.io/badge/Email-Direct%20Inquiry-red?style=flat&logo=gmail" />
  </a>
  <a href="https://wa.me/201014809916">
    <img src="https://img.shields.io/badge/WhatsApp-Connect-25D366?style=flat&logo=whatsapp" />
  </a>
</p>
