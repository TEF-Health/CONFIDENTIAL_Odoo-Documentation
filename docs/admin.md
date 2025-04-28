# Admin Guide

## Permission Management

### CSV Export

Admins can grant users to download the entire Odoo record as CSV.

!!! danger "Access to confidential information"
    The CSV export permission may only be granted to authorized users as it gives access to the full Odoo data record.
    
1. Activate Developer Mode by opening the General Settings page [https://tef.charite.de/odoo/settings](https://tef.charite.de/odoo/settings), scrolling to the bottom and clicking on **Activate the developer mode**.
2. Open the User Settings Page [https://tef.charite.de/odoo/users](https://tef.charite.de/odoo/users) and click on the user.
3. In the tab **Access Rights** scroll to **TECHNICAL** and select **Access to export feature**.  ![Export CSV](img/admin-export-csv.png)
    
    
## CSV Export

1. Go to Front Office Tab (Portal Backend) ![1](img/admin-csv-1.png).
2. Select List view and (optional) deselect the My assignments filter to see all applications. ![Export CSV](img/admin-csv-2.png).
3. Select all applications to download and press “Actions" and “Export” ![2](img/admin-csv-3.png).
4. **Select fields relevant for analysis**: By pressing the plus button on the left side, add the fields to a column in the exported spreadsheet. If selection is completed, press export. ![3](img/admin-csv-4.png).
5. Optional: Save selection as download template: This will save your selection so you do not have to put together all relevant fields again. ![4](img/admin-csv-5.png).
