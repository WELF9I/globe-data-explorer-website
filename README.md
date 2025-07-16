# 🌍 GlobeData Explorer API

**Your Gateway to Comprehensive Global Country Data**

## 🔍 Overview

GlobeData Explorer API is the most comprehensive and developer-friendly solution for accessing detailed country information. Whether you're building a travel app, conducting academic research, analyzing global markets, or integrating location-based features, our API delivers everything you need with exceptional performance and reliability.

<img width="1899" height="957" alt="Capture d’écran_2025-07-16_22-58-37" src="https://github.com/user-attachments/assets/9d657cbc-9523-4cf3-96dc-b0ff3916ec5b" />
<img width="1897" height="959" alt="Capture d’écran_2025-07-16_22-58-58" src="https://github.com/user-attachments/assets/9c26ff41-4507-421e-9b61-87194a380741" />
<img width="1899" height="956" alt="Capture d’écran_2025-07-16_22-59-17" src="https://github.com/user-attachments/assets/23847312-7da6-4123-b4aa-bd2deaa69a58" />


**Why choose GlobeData Explorer over other APIs?**

✅ **Rich Data**: 14+ fields, including flag emojis and neighbors  
✅ **Fast Access**: Optimized for quick responses  
✅ **Free to Start**: No credit card needed for the free tier  
✅ **Interactive Docs**: Explore at [Swagger UI](https://globe-data-api.onrender.com/docs)  
✅ **Community-Driven**: Suggest features via RapidAPI!

## 🚀 Quick Start

```bash
curl --request GET \
  --url https://globedata-explorer.p.rapidapi.com/countries/CN \
  --header 'x-rapidapi-host: globedata-explorer.p.rapidapi.com' \
  --header 'x-rapidapi-key: YOUR_API_KEY'
```

## 📊 Feature Comparison

| Feature                | GlobeData Explorer | Competitor A | Competitor B  |
|------------------------|--------------------|--------------|---------------|
| Free Tier              | ✅ Yes             | ❌ No        | ✅ Yes        |
| Data Fields            | 📋 14+             | 📋 8-10      | 📋 10-12      |
| Filtering Options      | ✅ Continent       | ❌ None      | ✅ Continent  |
| Flag Emojis            | ✅ Included        | ❌ Missing   | ❌ Missing    |
| Neighbor Countries     | ✅ Included        | ❌ Missing   | ❌ Partial    |
| OpenAPI Documentation  | ✅ Complete        | ❌ Partial   | ✅ Complete   |
------------------------------------------------------------------------------
## 🌟 Key Features

### Comprehensive Country Data
Access detailed information for every recognized country including:
- ISO 2-letter and 3-letter codes
- Official names and capitals
- Population statistics and land area
- Continent classifications
- Currency details (code and name)
- International phone codes
- Official languages
- Neighboring countries
- Flag emojis

### Powerful Querying
- **Pagination support** - Control result sets with `page` and `limit` parameters
- **Continent filtering** - Get only countries from specific continents
- **Fast lookups** - Find countries by ISO or ISO3 codes

### Developer Friendly
- **Clean RESTful API** - Predictable endpoints and responses
- **TypeScript definitions** - Available for all responses
- **Thorough documentation** - With interactive examples
- **Structured errors** - Helpful error messages and codes

## 📚 API Endpoints

### 1. Get All Countries
```
GET /countries
```
**Parameters:**
- `page` - Page number (default: 1)
- `limit` - Items per page (default: 10, max: 250)
- `continent` - Filter by continent code (e.g., "EU", "AS")

**Example Response:**
```json
{
  "data": [
    {
      "iso_code": "CN",
      "iso3_code": "CHN",
      "name": "China",
      "capital": "Beijing",
      "area_sq_km": 9596960,
      "population": 1411778724,
      "continent_code": "AS",
      "tld": ".cn",
      "currency_code": "CNY",
      "currency_name": "Yuan Renminbi",
      "phone_code": "86",
      "languages": ["zh-CN", "yue", "wuu"],
      "neighbours": ["LA", "BT", "TJ", "KZ"],
      "flag_emoji": "🇨🇳"
    }
  ],
  "pagination": {
    "total": 195,
    "page": 1,
    "limit": 1,
    "total_pages": 195
  }
}
```

### 2. Get Single Country
```
GET /countries/{code}
```
Find country by ISO 2-letter or 3-letter code

**Example:**
```bash
curl https://globedata-explorer.p.rapidapi.com/countries/US
```

### 3. Get Continents
```
GET /countries/continents
```
List all available continents with codes and names

## 🛠️ Integration Guides

### JavaScript
```javascript
const options = {
  method: 'GET',
  headers: {
    'x-rapidapi-host': 'globedata-explorer.p.rapidapi.com',
    'x-rapidapi-key': 'YOUR_API_KEY'
  }
};

fetch('https://globedata-explorer.p.rapidapi.com/countries/US', options)
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(err => console.error(err));
```

### Python
```python
import requests

url = "https://globedata-explorer.p.rapidapi.com/countries/US"

headers = {
    "x-rapidapi-host": "globedata-explorer.p.rapidapi.com",
    "x-rapidapi-key": "YOUR_API_KEY"
}

response = requests.get(url, headers=headers)
print(response.json())
```

## 💳 Pricing Plans

| Plan        | Requests/month | Price   | Features                  |
|-------------|----------------|---------|---------------------------|
| BASIC       | 1,000          | $0      | Basic access              |
| PRO         | 100,000        | $5.99   | Higher limits             |
| ULTRA       | 500,000        | $29.99  | Priority support          |


## ❓ Frequently Asked Questions

**Q: How often is the data updated?**  
A: Our database is updated quarterly to ensure accuracy.

**Q: Is there requests limiting?**  
A: Yes, free tier is limited to 1000 requests/month. Higher tiers have increased limits.

**Q: Can I request new features?**  
A: Absolutely! Contact us via RapidAPI or Email.

**Q: How do I get an API key?**  
A: Simply subscribe to any plan on RapidAPI to get your key instantly.

## 📬 Contact Us

Have questions or need help?  
📧 Email: welfkimedamine@gmail.com 
💬 RapidAPI: Message through our profile  

---

**Start building with the world's most comprehensive country data API today!**  
[Subscribe on RapidAPI](https://rapidapi.com/WELF9I/api/globedata-explorer)
