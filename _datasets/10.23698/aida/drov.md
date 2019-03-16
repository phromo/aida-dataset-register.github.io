---
datacite:
  "@context": "http://schema.org"
  "@type": "Dataset"
  "@id": "https://doi.org/10.23698/aida/drov"
  name: "Ovary data from the Visual Sweden project DROID"
  publicationYear: 2019
  about: "Pathology"
  url: "https://doi.aida.medtech4health.se/10.23698/aida/drov"
  author:
    - name: "Karin Lindman"
      "@id": "https://orcid.org/0000-0003-1298-517X"
      "@type": "Person"
      givenName: "Karin"
      familyName: "Lindman"
    - name: "Jerónimo F. Rose"
      "@id": "https://orcid.org/0000-0003-3845-8546"
      "@type": "Person"
      givenName: "Jerónimo"
      familyName: "Rose"
    - name: "Martin Lindvall"
      "@id": "https://orcid.org/0000-0002-7014-8874"
      "@type": "Person"
      givenName: "Martin"
      familyName: "Lindvall"
    - name: "Caroline Bivik Stadler"
      "@id": "https://orcid.org/0000-0001-7250-234X"
      "@type": "Person"
      givenName: "Caroline"
      familyName: "Bivik Stadler"
  publisher:
    "@type": "Organization"
    name: "AIDA"
  copyrightYear: 2019
  copyrightHolder:
    - "@type": "Organization"
      name: "Linköping University"
      url: "https://liu.se/"
    - name: "Claes Lundström"
      "@id": "https://orcid.org/0000-0002-9368-0177"
      "@type": "Person"
      givenName: "Claes"
      familyName: "Lundström"
  provider:
    - name: "Karin Lindman"
      email: "Karin.Lindman@regionostergotland.se"
      "@id": "https://orcid.org/0000-0003-1298-517X"
      "@type": "Person"
    - name: "Claes Lundstrom"
      email: "claes.lundstrom@liu.se"
      "@id": "https://orcid.org/0000-0002-9368-0177"
      "@type": "Person"
    - name: "Caroline Bivik Stadler"
      email: "caroline.bivik.stadler@liu.se"
      "@id": "https://orcid.org/0000-0001-7250-234X"
      "@type": "Person"
    - name: "Joel Hedlund"
      email: "joel.hedlund@liu.se"
      "@id": "https://orcid.org/0000-0001-6443-3604"
      "@type": "Person"
  dateCreated: "2019-01-09"
  datePublished: "2019-01-09"
  dateModified: "2019-01-09"
  keywords: "Pathology, Ovary, Cancer, Whole slide imaging, Annotated"
  version: "1.0"
  description: |
    This dataset consists of 174 WSI ovary whole slide images (WSI): 158
    malignant and 16 benign. Eight of the most common, histological definable
    tumour types were annotated: high grade serous carcinoma (HGSC), low grade
    serous carcinoma (LGSC), clear cell carcinoma (CC), endometrioid
    adenocarcinoma (EN), metastastic serous carcinoma (MS), metastatic other
    (MO), serous borderline tumor (SB) and mucinous borderline tumor (MB). Also
    normal ovarian tissue were annotated. 11258 separate annotations were made.
    For the benign structures only the epithelial structures, stroma and support
    tissue were annotated.
  rightsList:
    - rights: "Restricted access"
      rightsUri: "#license"
  citation:
    #- "@type": "CreativeWork"
    #  "@id": "https://doi.org/..."
    #  name: "Title of paper goes here"
other:
  status: "Completed"
  annotation: |
    One physician was responsible for the manual annotations controlled by a second
    pathologist.

    Eight of the most common, histological definable tumour types were
    annotated: high grade serous carcinoma (HGSC), low grade serous carcinoma
    (LGSC), clear cell carcinoma (CC), endometrioid adenocarcinoma (EN),
    metastastic serous carcinoma (MS), metastatic other (MO), serous borderline
    tumor (SB) and mucinous borderline tumor (MB). Also normal ovarian tissue
    was annotated. In total 11258 separate annotations were made. For the
    benign structures only the epithelial structures, stroma and support tissue
    were annotated.
  ethicsApproval: |
    The data collection and sharing is ethical approved.
  license: "#license"
  download:
    links:
      - text: ""
        url: ""
  organ:
    - name: "Ovary"
      sctid: 15497006 # SNOMED-CT https://termbrowser.nhs.uk/?perspective=full&conceptId1=%s
  age-span: "17-86 years"
  bytes: 108589866647
  numberOfImages: 174
  numberOfAnnotations: 11258
  resolution: "20X single plane"
  modality:
    - "Scanscope AT (Aperio, US)"
    - "NanoZoomer XR (Hamamatsu, Japan)" # FIXME: is this same as "Hamamatsu NanoZoomer-XR C12000 series 2013"?
    - "NanoZoomer XRL (Hamamatsu, Japan)" # FIXME: is this same as "Hamamatsu NanoZoomer 2.0 HT C9600 series 2013"
  stain: "H&E (hematoxylin and eosin)"
  phase:
  exampleImage:
  - title: "Overview of whole slide imaging."
    url: "/assets/images/10.23698/aida/drov/wsi.jpeg"
    thumbnail-url: "/assets/images/10.23698/aida/drov/wsi-thumbnail.jpeg"
  - title: "Overview of annotations."
    url: "/assets/images/10.23698/aida/drov/annotations.jpeg"
    thumbnail-url: "/assets/images/10.23698/aida/drov/annotations-thumbnail.jpeg"
  - title: "Detail view of annotations."
    url: "/assets/images/10.23698/aida/drov/detail.jpeg"
    thumbnail-url: "/assets/images/10.23698/aida/drov/detail-thumbnail.jpeg"
  - title: "To-scale view of pixel resolution in original whole slide imaging data."
    url: "/assets/images/10.23698/aida/drov/to-scale.jpeg"
    thumbnail-url: "/assets/images/10.23698/aida/drov/to-scale-thumbnail.jpeg"
---
## License
Copyright {{ page.datacite.copyrightYear }} {{ page.datacite.copyrightHolder | map: "name" |  join: ", " }}

Permission to use, copy, modify, and/or distribute this data within Analytic
Imaging Diagnostics Arena ([AIDA](https://medtech4health.se/aida)) for any
purpose with or without fee is hereby granted, provided that the above copyright
notice and this permission notice appear in all copies, and that publications
resulting from the use of this data cite the following works:

{{ page.datacite.author | map: "name" | array_to_sentence_string }} ({{ page.datacite.publicationYear }}) {{ page.datacite.name }} [doi:{{ page.datacite['@id'] | remove: "https://doi.org/" }}]({{ page.datacite["@id"] }}).

THE DATA IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD
TO THIS DATA INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN
NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR
CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA
OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR CHARACTERISTICS OF THIS
DATA.