---
hidden: no
datacite:
  dataset_id: adre-dafde
  "@context": "http://schema.org"
  "@type": "Dataset"
  "@id": 
  name: "Skin data"
  yearPublished: "2019"
  keywords: "Pathology, Whole slide imaging, Breast, Lymph nodes, Cancer, Sentinel nodes, Immunohistochemical staining, cytokeratin, CKAE1/AE3"
  version: v1.0.2 
  description: "The dataset consists of 99 H&E-stained whole slide skin images (WSI) - 49 abnormal and 50 normal cases. All significant abnormal findings identified are outlined and categorized into 13 types such as actinic keratosis, basal cell carcinoma and dermatofibroma. Other tissue components, such as epidermis, adnexal structures, as well as the surgical margin are delineated to create a complete histological map. In total, 16741 separate annotations have been made to segment the different tissue structures and link them to ontological information."

  license:
  - name: "Controlled access"
    id: "https://datahub.bp.mock.se/mock#controlled-access"
    "@type": "CreativeWork"
    abstract: |
      Free for use in legal and ethical medical diagnostics research.
  - name: "Big picture license"
    id: "https://"
  citation: Karin Lindman, Jerónimo F. Rose, Martin Lindvall, and Caroline Bivik Stadler (2019), Skin data. Big Picture doi:10.0001/adre-dafde.
  references: 
  - Stadler, C.B., Lindvall, M., Lundström, C. et al. Proactive Construction of an Annotated Imaging Database for Artificial Intelligence Training. J Digit Imaging (2020). https://doi.org/10.1007/s10278-020-00384-4
  access_time: Unlimited time
other:
  diagnosis: "Actinic keratosis, basal cell carcinoma, dermatofibroma, dysplastic nevus, intradermal nevus, keratoachantoma, lentigo malignant melanoma, malignant melanoma, malignant melanoma in situ, scar, seborrheic keratosis, squamous cell carcinoma and squamous cell carcinoma in situ + benign cases"

  geographical_area: Europe
  number_of_images: 150
  number_of_cases: 100
  number_of_biological_beings: 50
  number_of_observations: 
  comments: "One physician was responsible for the manual annotations controlled by a second pathologist. Accurate annotations were made over the whole tissues. 16741 separate annotations were made."
  metadata_version: v0.1.2
  changelog: "1.1.0 The benign images in the dataset were annoteted."
  center_name: Region Ostergotland, Sweden
  doi: 10.0001/adre-dafde
  age_at_extraction:
  - '45'
  - '90'
  anatomical_site:
  - Skin 39937001
  animal_species:
  - Homo sapiens
  block_preparation: []
  bp_image_type:
  - WSI Brightfield
  extraction_method:
  - Biopsy
  - Excision
  image_resolution:
  - 0.00022984807042544878
  - 0.00046104195481788847
  indirect_access_only: 'False'
  specimen_type:
  - Histopathology
  staining_name:
  - "H&E"
  shortName: "SD1"
  status:
  annotation: "YES. Manual annotations made by 1 resident reviewed by 1 pathologist. Accurate annotations were made over the whole tissues. 16741 separate annotations were made."
  countries-shared:
  - "FI"
  - "NO"
  - "SE"
  organ:
  age-span: "-"
  bytes: 5,497,558,138,880
  numberOfScans:
  numberOfAnnotations:
  modality: Immunohistochemistry
  scanner:
  - Aperio ScanScope AT
  - Hamamatsu NanoZoomer XR
  - Hamamatsu NanoZoomer S360
  - Hamamatsu NanoZoomer S60
  image: "/assets/images/mock_datasets/bp/m_p_b/ckae-metastasis-thumbnail.jpeg"
  exampleImage:
  - title: "Overview of whole slide imaging with hematoxylin and eosin staining."
    url: "/assets/images/mock_datasets/bp/m_p_b/he-overview.jpeg"
    thumbnail-url: "/assets/images/mock_datasets/bp/m_p_b/he-overview-thumbnail.jpeg"
  - title: "Overview of whole slide imaging with cytokeratin immunostaining."
    url: "/assets/images/mock_datasets/bp/m_p_b/ckae-overview.jpeg"
    thumbnail-url: "/assets/images/mock_datasets/bp/m_p_b/ckae-overview-thumbnail.jpeg"
  - title: "Detail view of metastasis with hematoxylin and eosin staining."
    url: "/assets/images/mock_datasets/bp/m_p_b/he-metastasis.jpeg"
    thumbnail-url: "/assets/images/mock_datasets/bp/m_p_b/he-metastasis-thumbnail.jpeg"
  - title: "Detail view of metastasis with cytokeratin immunostaining."
    url: "/assets/images/mock_datasets/bp/m_p_b/ckae-metastasis.jpeg"
    thumbnail-url: "/assets/images/mock_datasets/bp/m_p_b/ckae-metastasis-thumbnail.jpeg"
access: Direct
---

