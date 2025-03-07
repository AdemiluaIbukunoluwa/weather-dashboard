# WEATHER DASHBOARD

## Overview
A weather dashboard that fetches data from a weather API, stores it in an Amazon S3 bucket, and retrieves the data for display.

![weather-dashboard drawio](https://github.com/user-attachments/assets/af599166-3c0c-4c6f-b44c-c4a884da9dbd)


It combines the following DevOps principles:
- External API Integration (OpenWeather API)
- Cloud Storage (AWS S3)
- Infrastructure as Code
- Version Control (Git)
- Python Development
- Error Handling
- Environment Management

## Features
- Fetches real-time weather data for multiple cities
- Displays temperature (°F), humidity, and weather conditions
- Automatically stores weather data in AWS S3
- Supports multiple city tracking
- Timestamps all data for historical tracking

## Technical Architecture
- Language: Python
- API: OpenWeather API
- Cloud Provider: AWS
- boto3 (AWS SDK)
- python-dotenv
- requests

## Project Structure
```markdown
weather-dashboard/
  src/
    __init__.py
    weather_dashboard.py
  tests/
  data/
  .env
  .gitignore
  requirements.txt
```
## Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/AdemiluaIbukunoluwa/weather-dashboard.git

2. Install dependencies:
  pip install -r requirements.txt

3. Configure environment variables (in the .env file):
  OPENWEATHER_API_KEY=api_key
  AWS_BUCKET_NAME=bucket_name

4. Configure AWS credentials:
  aws configure

5. Run the application:
  python src/weather_dashboard.py

### Lessons Learned
- Gained hands-on experience with API integration and data handling
- Understood the process of storing and retrieving data from AWS S3 buckets
- Learned how to implement appropriate user policies for the S3 bucket to ensure secure access control
- Environment variable management for secure API keys
- Git workflow for project development
- Error handling in distributed systems
- Cloud resource management

Future Enhancements
- Create automated testing
- Set up CI/CD pipeline
- Add weather forecasting
- Implement data visualization
