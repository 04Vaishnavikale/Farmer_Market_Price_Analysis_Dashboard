# 🌾 Farmer Market Price Analysis Dashboard

## 📌 Project Overview
An interactive Power BI dashboard analyzing 
agricultural commodity prices across 6 major 
Indian APMC markets from January 2024 to 
May 2026. Built to help farmers, traders, and 
analysts track price trends, compare crops, 
and make data-driven decisions.

## 🎯 Objective
To monitor price fluctuations, identify seasonal 
trends, and compare prices across different 
markets and crops using interactive visuals 
and filters.

## 📊 Dashboard Features
### KPI Cards
- Average Market Price (₹)
- Minimum Price (₹)
- Maximum Price (₹)
- Price Range (₹)
- Total Arrivals
- Price Growth %

### Visualizations
- 📈 Price Trend Line Chart (2024-2026)
- 📊 Crop Price Comparison Bar Chart
- 🗺️ Market wise Price Distribution Map
- 🔽 Interactive Slicers (Crop/Year/Market)

### Advanced Features
- 🔍 Drill Through Pages (Crop Detail)
- 🧮 DAX Calculated Measures
- 🔧 Power Query Data Transformations

## 🧮 DAX Measures
- Avg Market Price = AVERAGE(Market_Price_Data[Avg_Price])
- Price Range = MAX(Market_Price_Data[Max_Price]) - MIN(Market_Price_Data[Min_Price])
- Total Arrivals = SUM(Market_Price_Data[Arrivals_Qty])
- Price Growth % = ROUND(DIVIDE(AVERAGE(Market_Price_Data[Avg_Price]),MIN(Market_Price_Data[Min_Price])) * 100, 2)

## 🔧 Power Query Transformations
- Verified all column data types
- Removed unnecessary Unit column
- Added Price Category column
  - Low  → Avg Price below ₹25
  - Medium → Avg Price ₹25-50
  - High → Avg Price above ₹50

## 📁 Dataset Details
| Field            | Details |
| Total Records    | 4,960 rows |
| Time Period      | Jan 2024 - May 2026 |
| Update Frequency | Weekly |
| Price Unit       | ₹ (Indian Rupee) |

## 🌾 Crops Covered
| Crop    | Unit      | Category |
| Mango   | kg        | High |
| Chili   | kg        | High |
| Rice    | quintal   | Medium |
| Banana  | dozen     | Medium |
| Carrot  | kg        | Medium |
| Tomato  | kg        | Medium |
| Onion   | kg        | Medium |
| Wheat   | quintal   | Medium |
| Potato  | kg        | Low |
| Cabbage | kg        | Low |

## 🗺️ Markets Covered
| Market                 | State |
| Mumbai APMC            | Maharashtra |
| Delhi Azadpur          | Delhi |
| Chennai Koyambedu      | Tamil Nadu |
| Kolkata Koley          | West Bengal |
| Bangalore Yeshwanthpur | Karnataka |
| Pune Market Yard       | Maharashtra |

## 📈 Key Insights
- 🥭 Mango is highest priced crop (~₹82)
- 🥬 Cabbage is most affordable crop (~₹20)
- 📈 Overall 12% price inflation (2024-2026)
- 🏙️ Chennai shows highest market prices
- 📦 Total 13.5M arrivals across all markets

## 🛠️ Tools & Technologies
| Tool             | Purpose |
| Power BI Desktop | Dashboard Development |
| Power Query      | Data Cleaning |
| DAX              | Calculated Measures |
| MS Excel         | Dataset Storage |
| GitHub           | Version Control |

## 📂 Repository Structure
farmer-market-dashboard/
│
├── Farmer_Market_Dashboard.pbix
│   └── Complete Power BI project
│
├── dashboard_preview.png
│   └── Dashboard screenshot
│
└── README.md
└── Project documentation

## 🚀 How to Use
1. Download `Farmer_Market_Dashboard.pbix`
2. Open with Power BI Desktop (Free)
3. Explore dashboard with slicers
4. Right click any crop → Drill Through
5. View Crop Detail page

## 👨‍💻 Author
## 🚀 How to Use
1. Download - Farmer_Market_Dashboard.pbix`
2. Open with Power BI Desktop (Free)
3. Explore dashboard with slicers
4. Right click any crop → Drill Through
5. View Crop Detail page

## 👨‍💻 Author
Vaishnavi
