---
hidden: no
datacite:
  "@context": "http://schema.org"
  "@type": "Dataset"
  "@id": 
  name: "Skin data"
  yearPublished: "2019"
  keywords: "Pathology, Whole slide imaging, Breast, Lymph nodes, Cancer, Sentinel nodes, Immunohistochemical staining, cytokeratin, CKAE1/AE3"
  version: v1.0.2 
  description: |
    Whole slide imaging of 150 full cases of skin.
    cancer cases. 
  license:
  - name: "Controlled access"
    id: "https://datahub.bp.mock.se/mock#controlled-access"
    "@type": "CreativeWork"
    abstract: |
      Free for use in legal and ethical medical diagnostics research.
  - name: "Big picture license"
    id: "https://"
  citation: Karin Lindman, Jerónimo F. Rose, Martin Lindvall, and Caroline Bivik Stadler (2019), Skin data. Big Picture doi:10.23698/aida/drsk.
  references: 
  - Stadler, C.B., Lindvall, M., Lundström, C. et al. Proactive Construction of an Annotated Imaging Database for Artificial Intelligence Training. J Digit Imaging (2020). https://doi.org/10.1007/s10278-020-00384-4
  access_time: Unlimited time
other:
  diagnosis: Actinic keratosis, basal cell carcinoma and, dermatofibroma + benign cases
  geographical_area: Europe
  number_of_images: 150
  number_of_cases: 100
  number_of_biological_beings: 2
  number_of_observations: 50
  comments: "One physician was responsible for the manual annotations controlled by a second pathologist. Accurate annotations were made over the whole tissues. 16741 separate annotations were made."
  metadata_version: v0.1.2
  changelog: "1.1.0 The benign images in the dataset were annoteted."
  center_name: Region Ostergotland, Sweden
  age_at_extraction:
  - '45'
  - '90'
  anatomical_site:
  - Skin structure of cheek (body structure)
  - Skin structure of upper arm
  - Skin structure of lower leg (body structure)
  - Skin structure of back (body structure)
  - Skin structure of hand (body structure)
  - Skin appendage structure
  - Skin of knee
  animal_species:
  - Homo sapiens
  block_preparation: []
  bp_image_type:
  - Brightfield
  extraction_method:
  - Biopsy
  - Scraping
  - Excision
  image_resolution:
  - 0.00022984807042544878
  - 0.00046104195481788847
  indirect_access_only: 'False'
  specimen_type:
  - Histopathology
  staining_name:
  - "KIR\xD6D" 
  - KI67
  - P16
  - hematoxylin stain,water soluble eosin stain
  - "SOXR\xD6D"
  - CK18
  - MELAN
  - HSV1
  - HSV2
  - CKAE
  - SOX10
  - HMB,
  shortName: "SD1"
  status:
  annotation: "YES"
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
## File formats
### Pixel position scaling
Coordinates given are relative to the image *width*. To get the correct pixel
position, X coordinates (and Y coordinates!) should therefore be multiplied with
the image *width*.

## License

Copyright
{{ page.datacite.copyrightYear }}
{{ page.datacite.copyrightHolder | map: "name" |  join: ", " }}

Donec nibh elit, tincidunt eget vulputate ac, consequat in ipsum. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Cras interdum enim at libero sodales finibus. Donec vitae lorem quam. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Phasellus eget orci vulputate quam porttitor dignissim. Maecenas commodo, nibh et iaculis blandit, leo arcu scelerisque tortor, id porttitor metus tortor commodo quam. Vivamus a dapibus ipsum, eu euismod elit.

{{ page.datacite.author | map: "name" | array_to_sentence_string }}
({{ page.datacite.datePublished | date: "%Y" }})
{{ page.datacite.name }}
[doi:{{ page.datacite['@id'] | remove: "https://doi.org/" }}]({{ page.datacite["@id"] }}).

 Integer tempus ullamcorper quam, eu consequat ante pulvinar ac. Nulla in ipsum mattis, congue orci vitae, rhoncus lacus. Aliquam nunc turpis, tincidunt in nibh eu, bibendum luctus diam. Praesent varius orci erat, nec sollicitudin tellus venenatis vel. Morbi quis ullamcorper arcu, quis ultricies odio.
