# Satellite Image Classification with DINOv2

An end-to-end computer vision pipeline that fine-tunes Meta's **DINOv2** foundation model to classify Sentinel-2 satellite imagery into 10 distinct land cover classes using the EuroSAT dataset.

---

## About the Project

Earth Observation (EO) data is vital for understanding environmental shifts, urban growth, and agricultural production. However, manual analysis of satellite imagery is time-consuming and difficult to scale. 

This project adapts Meta’s **DINOv2** (`facebook/dinov2-base`) Vision Transformer (ViT) architecture to automate land-use and land-cover (LULC) classification. Built with PyTorch and Hugging Face Transformers, the training workflow features automated checkpointing to guarantee seamless recovery across interrupted sessions.

### Real-World Applications
* **Environmental Monitoring:** Tracking deforestation rates, wetland preservation, and water-body variations over time.
* **Urban Planning & Development:** Monitoring city expansion, identifying residential zones, and infrastructure density.
* **Precision Agriculture:** Classifying farmland, mapping crop types, and analyzing seasonal vegetation patterns.
* **Disaster Management:** Rapidly mapping roads, industrial zones, and surrounding terrain following floods or fires.

---

## Dataset

This project uses the **EuroSAT** dataset (RGB format) derived from Sentinel-2 satellite imagery.

* **Source:** [EuroSAT Dataset on Kaggle](https://www.kaggle.com/datasets/apollo2506/eurosat-dataset)
* **Classes (10):**
  1. `AnnualCrop`
  2. `Forest`
  3. `HerbaceousVegetation`
  4. `Highway`
  5. `Industrial`
  6. `Pasture`
  7. `PermanentCrop`
  8. `Residential`
  9. `River`
  10. `SeaLake`