---
datacite:
  "@context": "http://schema.org"
  "@type": "Dataset"
  "@id": "https://doi.org/10.23698/aida/drli"
  name: "Liver data from the Visual Sweden project DROID"
  publicationYear: 2019
  about: "Pathology"
  url: "https://doi.aida.medtech4health.se/10.23698/aida/drli"
  author:
    - name: "Mischa Woisetschläger"
      "@id": "https://orcid.org/0000-0003-0066-4985"
      "@type": "Person"
    - name: "Johan Blomma"
      "@id": "" # FIXME: missing info
      "@type": "Person"
    - name: "Nils Dahlström"
      "@id": "https://orcid.org/0000-0002-4111-1693"
      "@type": "Person"
    - name: "Caroline Bivik Stadler"
      "@id": "https://orcid.org/0000-0001-7250-234X"
      "@type": "Person"
    - name: "Daniel Forsberg"
      "@id": "https://orcid.org/0000-0003-0908-9470"
      "@type": "Person"      
  publisher:
    "@type": "Organization"
    name: "AIDA"
  copyrightYear: 2019
  copyrightHolder:
    - name: "Linköping University"
      "@type": "Organization"
      url: "https://liu.se/"
    - name: "Claes Lundström"
      "@id": "https://orcid.org/0000-0002-9368-0177"
      "@type": "Person"
  provider:
    - name: "Anna Bodén"
      email: "Anna.C.Boden@regionostergotland.se"
      "@id": "https://orcid.org/0000-0002-0128-870X"
      "@type": "Person"
    - name: "Claes Lundstrom"
      email: "claes.lundstrom@liu.se"
      "@id": "https://orcid.org/0000-0002-9368-0177"
      "@type": "Person"
    - name: "Joel Hedlund"
      email: "joel.hedlund@liu.se"
      "@id": "https://orcid.org/0000-0001-6443-3604"
      "@type": "Person"
  dateCreated: "2019-01-09"
  datePublished: "2019-01-09"
  dateModified: "2019-01-09"
  keywords: "Radiology, Liver, Cancer, Computed tomography, Annotated"
  version: "1.0"
  description: |
    77 CT abdomen (computed tomography) examinations taken with contrast in
    venous phase. All cases showed liver malignancies. Manual oncological
    annotations were made by a radiologist and these were controlled by a second
    experienced radiologist. All changes with a diameter greater than 5mm were
    segmented and assumed metastases (cysts excluded as defined by HU). 317
    lesions were annotated.
  rightsList:
    - rights: "Restricted access"
      rightsURI: "#license"
  citation:
    #- "@type": "CreativeWork"
    #  "@id": "https://doi.org/..."
    #  name: "Title of paper goes here"
other:
  status: "Completed"
  annotation: |
    Manual oncological annotations was made by a radiologist and these were
    controlled by a second radiologist. All changes with a diameter greater than
    5mm was segmented and as assumed metastases (cysts excluded defined by HU).
    317 lesions were annotated.
  ethicsApproval: |
    The data collection and sharing is ethical approved.
  license: "#license"
  download:
    links:
      - text: ""
        url: ""
  organ:
    - name: "Liver"
      sctid: 10200004 # SNOMED-CT https://termbrowser.nhs.uk/?perspective=full&conceptId1=%s
  age-span:
  bytes: # FIXME: Missing info.
  numberOfImages: 77
  numberOfAnnotations: 317
  resolution:
  modality:
    - "Siemens CT Scanners"
  stain:
  phase: Venuous (with contrast)
  exampleImage:
    - title: "3D illustration of locations, sizes and distribution in liver metastasis (green)."
      url: "/assets/images/10.23698/aida/drli/3d.png"
      thumbnail-url: "/assets/images/10.23698/aida/drli/3d-thumbnail.png"
    - title: "Slice from thorax CT stack with annotated liver metastases."
      url: "/assets/images/10.23698/aida/drli/slice.jpeg"
      thumbnail-url: "/assets/images/10.23698/aida/drli/slice-thumbnail.jpeg"
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