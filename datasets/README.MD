
1. `detailed_df` - a dataset with detailed localities (suited for analyzing how many districts were affected during an alert).

- **Total rows:** 61281
- **Time column (`'time'`):** Converted to `datetime64[ns]` format  
- **Missing value** None  

**Columns:**

| Column Name | Description |
|-------------|------------|
| **datetime** | Date and time of the warning in `datetime64[ns]` format |
| **locality** | Name of the locality (city, town, or settlement) |
| **region** | Region to which the locality belongs |
| **threat_type** | Type of warning. Possible values: `'Red Alert'`, `'Unrecognized Aircraft'`, `'Terrorist Infiltration'`, `'Interception Pieces'`, `'Earthquake'` |
| **district** | Administrative district or region where the locality is located; an official governmental division. |

---

2. `df` - a dataset where zones of large cities are combined into a single record. It is suited for counting how many times an alert was triggered in certain cities and localities.

- **Total rows:** 57543
- **Time column (`'time'`):** Converted to `datetime64[ns]` format  
- **Missing value** None  

**Columns:**

| Column Name | Description |
|-------------|------------|
| **datetime** | Date and time of the warning in `datetime64[ns]` format |
| **locality** | Name of the locality (city, town, or settlement) |
| **zones** | Zones within a locality. If the locality is not a major city, this column contains `'All'` |
| **region** | Region to which the locality belongs |
| **threat_type** | Type of warning. Possible values: `'Red Alert'`, `'Unrecognized Aircraft'`, `'Terrorist Infiltration'`, `'Interception Pieces'`, `'Earthquake'` |
| **district** | Administrative district or region where the locality is located; an official governmental division. |


