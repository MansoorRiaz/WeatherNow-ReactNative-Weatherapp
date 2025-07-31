# WeatherNow - Modern Weather App

## 🌤️ Overview

WeatherNow is a sophisticated, feature-rich weather application built with React Native and Expo. It provides real-time weather data, location-based forecasts, and a beautiful, intuitive user interface that adapts to different weather conditions.

## ✨ Key Features

### 🌍 **Location-Based Weather**
- Automatic GPS location detection
- Real-time weather data for current location
- City search functionality with global coverage
- Saved cities management with quick access

### 📊 **Comprehensive Weather Data**
- **Current Weather**: Temperature, feels-like, humidity, wind speed/direction
- **Hourly Forecast**: 8-hour detailed forecast with precipitation probability
- **Weekly Forecast**: 7-day extended forecast with high/low temperatures
- **Weather Stats**: UV index, sunrise/sunset times, air quality index (AQI)
- **Additional Metrics**: Pollen levels, driving conditions, running conditions

### 🎨 **Dynamic UI/UX**
- **Weather-Adaptive Backgrounds**: Beautiful background images that change based on weather conditions
- **Smooth Animations**: Blur effects, slide animations, and haptic feedback
- **Modern Design**: Clean, minimalist interface with card-based layout
- **Responsive Layout**: Optimized for both mobile and tablet devices

### 📰 **Weather News Integration**
- Location-specific weather news
- Real-time news updates from reliable sources
- Horizontal scrolling news cards with direct links

### 🔧 **Advanced Features**
- **Multi-API Integration**: OpenWeatherMap, WeatherAPI, IQAir, NewsAPI, GeoDB
- **Offline City Management**: Save and manage favorite cities locally
- **Search Functionality**: Global city search with population-based sorting
- **Error Handling**: Robust error boundaries and fallback mechanisms

## 🛠️ Technology Stack

### **Frontend**
- **React Native** (0.79.5) - Cross-platform mobile development
- **Expo** (53.0.17) - Development platform and tools
- **TypeScript** - Type-safe development
- **React Navigation** - Navigation management

### **UI/UX Libraries**
- **Expo Blur** - Beautiful blur effects
- **React Native Reanimated** - Smooth animations
- **Expo Haptics** - Tactile feedback
- **Lottie React Native** - Animated weather icons

### **APIs & Services**
- **OpenWeatherMap API** - Primary weather data
- **WeatherAPI** - Secondary weather data and fallback
- **IQAir API** - Air quality and pollen data
- **NewsAPI** - Weather-related news
- **GeoDB Cities API** - Global city search
- **BigDataCloud** - Reverse geocoding

### **Development Tools**
- **ESLint** - Code linting and formatting
- **TypeScript** - Static type checking
- **Expo Router** - File-based routing

## 📱 Platform Support

- **iOS** - Native iOS app with tablet support
- **Android** - Native Android app with edge-to-edge support
- **Web** - Progressive web app (PWA) support
- **Cross-Platform** - Single codebase for all platforms

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn
- Expo CLI
- iOS Simulator (for iOS development)
- Android Studio (for Android development)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/WeatherNow.git
   cd WeatherNow
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure API Keys**
   Create a `config.ts` file in the root directory:
   ```typescript
   export const OPEN_WEATHER_API_KEY = "your_open_weather_api_key";
   export const GEODB_API_KEY = "your_geodb_api_key";
   export const NEWS_API_KEY = "your_news_api_key";
   export const IQAIR_API_KEY = "your_iqair_api_key";
   export const WEATHERAPI_KEY = "your_weatherapi_key";
   ```

4. **Start the development server**
   ```bash
   npm start
   ```

5. **Run on your preferred platform**
   - **iOS**: Press `i` in terminal or scan QR code with Expo Go
   - **Android**: Press `a` in terminal or scan QR code with Expo Go
   - **Web**: Press `w` in terminal or open browser

## 📋 API Keys Required

### OpenWeatherMap API
- **Purpose**: Primary weather data, forecasts, and air quality
- **Sign up**: [OpenWeatherMap](https://openweathermap.org/api)
- **Free tier**: 1,000 calls/day

### WeatherAPI
- **Purpose**: Secondary weather data and fallback
- **Sign up**: [WeatherAPI](https://www.weatherapi.com/)
- **Free tier**: 1,000,000 calls/month

### IQAir API
- **Purpose**: Air quality and pollen data
- **Sign up**: [IQAir](https://www.iqair.com/air-pollution-data-api)
- **Free tier**: 1,000 calls/day

### NewsAPI
- **Purpose**: Weather-related news articles
- **Sign up**: [NewsAPI](https://newsapi.org/)
- **Free tier**: 1,000 requests/day

### GeoDB Cities API
- **Purpose**: Global city search functionality
- **Sign up**: [RapidAPI GeoDB](https://rapidapi.com/wirefreethought/api/geodb-cities/)
- **Free tier**: 1,000 requests/month

## 🏗️ Project Structure

```
WeatherNow/
├── app/                    # Main application screens
│   ├── index.tsx          # Primary weather screen
│   ├── _layout.tsx        # App layout configuration
│   └── +not-found.tsx     # 404 error page
├── assets/                # Static assets
│   ├── images/           # App icons and weather images
│   ├── lottie/          # Animated weather icons
│   └── fonts/           # Custom fonts
├── components/           # Reusable UI components
├── constants/           # App constants and configurations
├── hooks/              # Custom React hooks
├── scripts/            # Build and utility scripts
└── config.ts           # API configuration (not in repo)
```

## 🎯 Key Components

### **Main Weather Screen** (`app/index.tsx`)
- **MainWeatherCard**: Current weather display with large temperature and conditions
- **HourlyForecastSection**: Horizontal scrolling hourly forecast
- **WeeklyForecastSection**: 7-day forecast with precipitation probability
- **WeatherNewsSection**: Location-specific weather news
- **WeatherStatsSection**: Detailed weather statistics and metrics

### **Interactive Features**
- **City Search Modal**: Global city search with real-time results
- **Drawer Menu**: Saved cities management with quick access
- **Weather-Adaptive UI**: Dynamic backgrounds and colors based on conditions
- **Error Boundaries**: Robust error handling and user feedback

## 🔧 Customization

### **Weather Backgrounds**
The app automatically changes background images based on weather conditions:
- **Clear**: Sunny yellow gradient
- **Clouds**: Gray gradient
- **Rain**: Blue gradient
- **Thunderstorm**: Dark gradient

### **Color Schemes**
Weather-adaptive color schemes that match current conditions:
- **Temperature Colors**: Warm colors for high temps, cool for low
- **Icon Colors**: Weather-appropriate icon coloring
- **Background Gradients**: Dynamic gradients based on weather type

## 📊 Performance Features

- **Optimized API Calls**: Efficient data fetching with fallback mechanisms
- **Image Caching**: Weather background images are cached locally
- **Lazy Loading**: Components load only when needed
- **Error Recovery**: Graceful handling of API failures
- **Offline Support**: Saved cities work without internet connection

## 🔒 Security & Privacy

- **API Key Management**: Secure configuration file (not in repository)
- **Location Permissions**: Explicit user consent for GPS access
- **Data Privacy**: No personal data collection or storage
- **HTTPS Only**: All API calls use secure connections

## 🐛 Troubleshooting

### Common Issues

1. **API Key Errors**
   - Ensure all API keys are correctly configured in `config.ts`
   - Check API key quotas and limits
   - Verify API key permissions

2. **Location Services**
   - Enable location permissions in device settings
   - Ensure GPS is enabled for accurate location
   - Check internet connectivity

3. **Build Issues**
   - Clear Expo cache: `expo r -c`
   - Reset Metro bundler: `npm start --reset-cache`
   - Update dependencies: `npm update`

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Make your changes and test thoroughly
4. Commit your changes: `git commit -m 'Add feature'`
5. Push to the branch: `git push origin feature-name`
6. Submit a pull request

## 📄 License

This project is licensed under a restrictive license. Please see the [LICENSE](LICENSE) file for details.

**You are not permitted to copy, modify, or distribute this software for any purpose, including commercial use.**

## 🙏 Acknowledgments

- **OpenWeatherMap** for comprehensive weather data
- **Expo** for the excellent development platform
- **React Native** community for the robust framework
- **WeatherAPI** for additional weather data sources
- **NewsAPI** for weather-related news content

## 📞 Support

For support, please open an issue on GitHub or contact the development team.

---

**WeatherNow** - Bringing weather information to your fingertips with style and precision! 🌤️
