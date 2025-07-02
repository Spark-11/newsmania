# News Summarizer

A modern news aggregator that uses AI to provide concise summaries of news articles from multiple Indian news sources.

## Demo



https://github.com/user-attachments/assets/0c184d88-71c9-4cea-ad07-b6e62c8aabb9




## Technologies Used

### Frontend
- React.js with Vite
- Tailwind CSS for styling
- Axios for API calls
- React Router DOM for routing
- Heroicons for beautiful icons

### Backend
- Node.js & Express.js
- MongoDB for data storage
- RSS Parser for fetching news feeds

### AI Service
- Python Flask API
- Hugging Face Transformers (mT5 model)
- CORS for cross-origin requests

## Setup Instructions

### Prerequisites
- Node.js (v14 or higher)
- Python 3.8 or higher
- MongoDB installed and running locally

### Installation

1. **Clone the repository**
```bash
git clone [repository-url]
cd news-summarizer
```

2. **Backend Setup**
```bash
cd server
npm install
# Create .env file with MongoDB URI
echo "MONGODB_URI=mongodb://localhost:27017/news-summarizer" > .env
npm start
```

3. **Frontend Setup**
```bash
cd client
npm install
npm run dev
```

4. **AI Service Setup**
- For the AI part, I take the help of Google Colab for using GPU Service, so that summarization takes place in less time.
```bash
https://colab.research.google.com/drive/1ZCHBnCn6v77_njD7iETcUtdkLFIZ3BR_?usp=sharing
```
- After running the code in Google Colab, paste the link found in the output in your .env file

## Features
- Real-time news fetching from multiple sources
- AI-powered article summarization
- Clean and modern UI with responsive design
- User can create their notes for a particular article
- Automatic refresh of news feed

## RSS Feed Sources
- ABP Live: https://news.abplive.com/news/india/feed
- Amar Ujala: https://www.amarujala.com/rss/breaking-news.xml

## Architecture
The application follows a microservices architecture with three main components:
1. React Frontend (Port 5173)
2. Express Backend (Port 3000)
3. Flask AI Service (Port 5000)
