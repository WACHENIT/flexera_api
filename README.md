# Flexera One Custom Reporting Template  
**Consumed Apps & Licenses**

## 📋 Overview  
This Policy Template (`.pt` JSON) for Flexera One automates extraction and formatting of consumed-app and license-usage data. It empowers your team to:

- 📊 Generate up-to-date usage dashboards  
- 📩 Email detailed CSV or PDF reports on schedule  
- 🔔 Alert on over- or under-utilized licenses  

## 🚀 Quickstart

1. **Import Template**  
   - In Flexera One UI, navigate to **Policy Management → Import Policy**  
   - Upload `consumed_apps_and_licenses.pt`  
2. **Configure OAuth2 Credentials**  
   - Create or reuse a **Refresh-Token** credential under **Automation → Credentials**  
   - Attach to this policy so it can request Access-Tokens automatically  
3. **Set Schedule**  
   - Under **Applied Policies**, choose **Run Schedule** (e.g. daily 02:00 UTC)  
   - Add recipient email addresses  

4. **Run & Verify**  
   - Click **Run Now** to validate  
   - Check **Events → Automation** for success/failure logs  
   - Download report from the email or via the Events details  

## 🛠️ Template Details  
- **Data Source**: Consumption metrics & license inventory  
- **Filters**: Active users, non-compliant usage thresholds  
- **Output**: CSV columns for App Name, User Count, Licenses Consumed, Compliance Status  

## 🔄 Maintenance  
- To adjust thresholds or columns, edit the `.pt` file in your local IDE and re-import.  
- Store updates in Git and tag releases (v1.0.0, v1.1.0, etc.).  
- Monitor token expiry in **Automation → Credentials**; refresh the token at least every 30 days.

## 📞 Support  
For issues or enhancement requests, please open a GitHub Issue or contact the License Management team at `lizenz@btc-ag.com`.  

---

*Built by Wassim Cheniti, BTC IT Services GmbH*  
