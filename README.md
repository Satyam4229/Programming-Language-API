# Programming Language API

This API provides information about various programming languages, including database languages, markup languages, and scripting languages. It is deployed on Render and can be accessed using the following endpoints.

## API Endpoints

### 1. Get All Programming Languages
**Endpoint:**
```http
GET https://programming-language-api.onrender.com/api/languages
```
**Description:**
Retrieves a list of all available programming languages with their details.

---

### 2. Get a Programming Language by Index
**Endpoint:**
```http
GET https://programming-language-api.onrender.com/api/languages/{index}
```
**Description:**
Retrieves the programming language at the specified index in the dataset.

**Example Request:**
```http
GET https://programming-language-api.onrender.com/api/languages/5
```

**Response:**
```json
{
  "name": "Python",
  "type": "Programming Language",
  "paradigm": "Object-Oriented, Functional, Procedural",
  "description": "Python is an interpreted, high-level programming language known for its simplicity and readability."
}
```

---

### 3. Get a Programming Language by Name
**Endpoint:**
```http
GET https://programming-language-api.onrender.com/api/languages/{language-name}
```
**Description:**
Retrieves details of a specific programming language by its name.

**Example Request:**
```http
GET https://programming-language-api.onrender.com/api/languages/python
```

**Response:**
```json
{
  "name": "Python",
  "type": "Programming Language",
  "paradigm": "Object-Oriented, Functional, Procedural",
  "description": "Python is an interpreted, high-level programming language known for its simplicity and readability."
}
```

---

## Setup and Deployment

### 1. Clone the Repository
```sh
git clone https://github.com/Satyam4229/Programming-Language-API.git
cd Programming-Language-API
```

### 2. Install Dependencies
```sh
pip install -r requirements.txt
```

### 3. Run the API Locally
```sh
python app.py
```

The API will be available at `http://127.0.0.1:5000`.

---

## Hosting on Render
This API is hosted on **Render** and can be accessed using the URLs mentioned in the **API Endpoints** section.

To deploy it on Render, follow these steps:
1. Push your latest code to GitHub.
2. Go to [Render](https://render.com/) and create a new **Web Service**.
3. Connect your GitHub repository.
4. Set the **Build Command**: `pip install -r requirements.txt`
5. Set the **Start Command**: `gunicorn app:app`
6. Deploy the service.

---

## Contributing
Feel free to contribute by submitting issues or pull requests on GitHub.

---

## License
This project is licensed under the **MIT License**.

---

## Contact
For any queries or suggestions, reach out via:
- GitHub: [Satyam4229](https://github.com/Satyam4229)
- Email: psatyam4229@gmail.com 


