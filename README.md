
# Mango Fusion App 

[**Live App**](https://mango-fusion-brown.vercel.app/) | [**Research Article**](https://rdcu.be/eRTRy) | [**Models on Hugging Face**](https://huggingface.co/mohsinramzan/mango_fusion_models)

---

## Table of Contents

- [Mango Fusion App](#mango-fusion-app)
  - [Table of Contents](#table-of-contents)
  - [Overview](#overview)
  - [Features](#features)
  - [Demo](#demo)
  - [Repository Structure](#repository-structure)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Dataset](#dataset)
  - [Models](#models)
  - [Research Files](#research-files)
  - [Contributing](#contributing)
  - [License](#license)

---

## Overview

Mango Fusion is a machine learning application for classifying mango diseases. It uses pretrained CNN models for individual leaf and fruit image classification and incorporates a novel dynamic attention-based fusion model that combines predictions from both modalities to enhance accuracy and improve generalizatio

This app is based on our published research: [Dual-modality fusion for mango 
disease classification using dynamic attention based ensemble of leaf & fruit images](https://rdcu.be/eRTRy).

---

## Features

- Predict mango diseases from **leaf images**  
- Predict mango diseases from **fruit images**  
- **Fusion-based prediction** combining leaf and fruit cues for enhanced accuracy  
- Supports multiple pretrained models:
  - ConvNeXt  
  - ResNet-50  
  - MobileNetV2  
  - EfficientNet-B0  
- Web-based interface for easy use  
- Backend powered by Django, deployed on Vercel  

---

## Demo

Access the live web application here: [https://mango-fusion-brown.vercel.app/](https://mango-fusion-brown.vercel.app/)

---

## Repository Structure


* `MangoDiseaseClassifier/` – Django project containing main backend logic
* `mango_fusion/` – Mango Fusion app files
* `Research_Files/` – Research and Experiment Juypter Notebooks
* `db.sqlite3` – SQLite database for the Django app
* `manage.py` – Django project management script
* `requirements.txt` – Python dependencies
* `vercel.json` – Deployment configuration for Vercel

---

## Installation

1. Clone the repository:

```bash
git clone https://github.com/mohsinwarind/Mango_Fusion.git
cd mango-fusion
```

2. Create a virtual environment:

```bash
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Run migrations:

```bash
python manage.py migrate
```

5. Start the development server:

```bash
python manage.py runserver
```

---

## Usage

* Upload a mango leaf , fruit image or both , through the web interface.
* Select the model for prediction.
* The app will display the predicted disease along with confidence scores.

---

## Dataset

The mango leaf and fruit dataset is **available upon request**. Contact: `mohsinramzan999@gmail.com`.

---

## Models

All pretrained models are hosted on Hugging Face:
[https://huggingface.co/mohsinramzan/mango_fusion_models](https://huggingface.co/mohsinramzan/mango_fusion_models)

Includes:

* Leaf-only models
* Fruit-only models
* Fusion models for leaf + fruit prediction

---

## Research Files

The `Research_Files` folder contains:


* Experiment scripts
* Data analysis notebooks

---

## Contributing

We welcome contributions! To contribute:

1. Fork the repository
2. Create a new branch (`git checkout -b feature-name`)
3. Make your changes and commit (`git commit -m "Description"`)
4. Push to your branch (`git push origin feature-name`)
5. Create a Pull Request

---

## License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

---

