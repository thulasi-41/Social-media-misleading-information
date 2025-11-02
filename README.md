# Social Media Misleading Information Detection System

## 📋 Overview

This project is a machine learning-based web application designed to detect and classify misleading information on social media platforms. Built with Django and Python, the system analyzes news articles and social media content to distinguish between genuine and fake information, helping users identify potentially misleading content.

## ✨ Features

- **Automated Detection**: Machine learning algorithms to classify news articles as genuine or fake
- **User-Friendly Interface**: Web-based dashboard for easy interaction
- **Real-time Analysis**: Quick processing and classification of social media content
- **Data Visualization**: Visual representation of analysis results
- **Historical Data**: Access to analyzed content and classification history
- **Multi-User Support**: Separate portals for service providers and end users
- **Secure Authentication**: User registration and login system

## 🛠️ Technology Stack

- **Backend Framework**: Django (Python)
- **Frontend**: HTML, CSS, JavaScript
- **Machine Learning**: Python ML libraries (scikit-learn, pandas, numpy)
- **Database**: SQLite/MySQL
- **Language**: Python 3.x

## 📁 Project Structure

```
Social-media-misleading-information/
├── social_mediaand_misleading_information/
│   ├── Remote_User/              # User interface and functionalities
│   ├── Service_Provider/         # Admin/service provider interface
│   ├── Template/                 # HTML templates
│   ├── social_mediaand_misleading_information/  # Django settings
│   └── manage.py                 # Django management script
├── Database/                     # Database files and schemas
├── .idea/                        # IDE configuration
├── DataStructure.txt             # Data structure documentation
└── README.md                     # Project documentation
```

## 🚀 Installation and Setup

### Prerequisites

- Python 3.7 or higher
- pip (Python package manager)
- Virtual environment (recommended)

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/thulasi-41/Social-media-misleading-information.git
   cd Social-media-misleading-information
   ```

2. **Create a virtual environment** (recommended)
   ```bash
   python -m venv venv
   
   # On Windows
   venv\Scripts\activate
   
   # On macOS/Linux
   source venv/bin/activate
   ```

3. **Install required dependencies**
   ```bash
   pip install -r requirements.txt
   ```
   
   If `requirements.txt` is not available, install the following packages:
   ```bash
   pip install django pandas numpy scikit-learn matplotlib seaborn
   ```

4. **Navigate to the project directory**
   ```bash
   cd social_mediaand_misleading_information
   ```

5. **Run database migrations**
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

6. **Create a superuser** (admin account)
   ```bash
   python manage.py createsuperuser
   ```

7. **Start the development server**
   ```bash
   python manage.py runserver
   ```

8. **Access the application**
   - Open your web browser and navigate to: `http://127.0.0.1:8000/`
   - Admin panel: `http://127.0.0.1:8000/admin/`

## 💻 Usage

### For End Users

1. **Register/Login**: Create an account or log in to the system
2. **Submit Content**: Enter news articles or social media content for analysis
3. **View Results**: Review the classification results (Genuine/Fake)
4. **Access History**: Check previously analyzed content

### For Service Providers

1. **Login**: Access the service provider portal
2. **Monitor System**: View overall system statistics and performance
3. **Manage Users**: Handle user accounts and permissions
4. **Review Classifications**: Analyze classification patterns and accuracy
5. **Train Model**: Update and retrain the machine learning model with new data

## 📊 Machine Learning Model

The system uses supervised machine learning algorithms to classify content:

- **Training Data**: Pre-labeled dataset of genuine and fake news articles
- **Features**: Text-based features extracted from content (TF-IDF, word frequencies, etc.)
- **Algorithms**: Multiple classifiers including:
  - Naive Bayes
  - Logistic Regression
  - Support Vector Machines (SVM)
  - Random Forest
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-Score

## 🗄️ Database Structure

The system uses a relational database with the following main entities:

- **Users**: User authentication and profile information
- **Articles**: Stored news articles and social media content
- **Classifications**: Classification results with timestamps
- **Training Data**: Labeled dataset for model training

For detailed database schema, refer to `DataStructure.txt`.

## 🔒 Security Considerations

- User passwords are hashed and securely stored
- CSRF protection enabled for all forms
- SQL injection prevention through Django ORM
- XSS protection for user-generated content
- Session management and authentication

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Create a Pull Request

## 📝 License

This project is open source. Please check the repository for specific license information.

## 👥 Authors

- **Thulasi** - [GitHub Profile](https://github.com/thulasi-41)

## 📧 Contact

For questions, suggestions, or issues, please open an issue on GitHub or contact the repository owner.

## 🙏 Acknowledgments

- Thanks to the open-source community for providing excellent tools and libraries
- Dataset sources for training the machine learning models
- Django framework for robust web application development

## 📚 Future Enhancements

- [ ] Integration with real-time social media APIs (Twitter, Facebook)
- [ ] Deep learning models for improved accuracy
- [ ] Multi-language support
- [ ] Mobile application
- [ ] Advanced visualization dashboards
- [ ] API endpoints for third-party integration
- [ ] Automated fact-checking with external sources
- [ ] Browser extension for real-time detection

## 🐛 Known Issues

Please refer to the [Issues](https://github.com/thulasi-41/Social-media-misleading-information/issues) page for known bugs and feature requests.

---

**Note**: This is an educational/research project. While the system aims to detect misleading information, it should not be the sole source for determining content authenticity. Always verify critical information through multiple reliable sources.
