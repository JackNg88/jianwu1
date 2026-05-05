---
# Homepage
type: landing

sections:
  # About / Biography
  - block: about.biography
    id: about
    content:
      title: Biography
      username: admin

  # Skills
  - block: skills
    id: skills
    content:
      title: Expertise
      username: admin
      text: ''
    design:
      columns: '1'

  # Experience
  - block: experience
    id: experience
    content:
      title: Experience
      date_format: Jan 2006
      items:
        - title: Researcher
          company: Center for Infection and Genomics of the Lung (CIGL), Justus Liebig University Giessen
          company_url: 'https://www.uni-giessen.de'
          location: Gießen, Germany
          date_start: '2023-02-01'
          date_end: ''
          description: |
            Research in lung infection genomics using single-cell and spatial transcriptomics approaches.

        - title: Research Assistant I
          company: Centre for Translational Stem Cell Biology & The University of Hong Kong
          company_url: 'https://www.hku.hk'
          location: Hong Kong
          date_start: '2021-12-01'
          date_end: '2023-02-28'
          description: |
            Under supervision of Prof. Pentao Liu.
            - Expanded potential stem cells (EPSCs) from human embryos
            - Single-cell RNA-seq analysis of EPSC differentiation toward TSCs
            - Molecular criteria for defining bovine, porcine and human EPSCs

        - title: Research Assistant I
          company: The University of Hong Kong
          company_url: 'https://www.hku.hk'
          location: Hong Kong
          date_start: '2019-05-01'
          date_end: '2021-12-31'
          description: |
            Under supervision of Prof. Pentao Liu.
            - Establishment of Bovine Expanded Potential Stem Cells
            - Decidual glycodelin-A and Siglec-7 macrophage polarization
            - Porcine and human EPSC establishment

        - title: Graduate Researcher
          company: Guangzhou Institutes of Biomedicine and Health (GIBH), Chinese Academy of Sciences
          company_url: ''
          location: Guangzhou, China
          date_start: '2015-09-01'
          date_end: '2018-06-30'
          description: |
            Under supervision of Prof. Duanqing Pei.
            - Transposable elements (TEs) from hES to liver
            - Cancer metastasis via circulating tumour cells (CTC)
            - Chromatin accessibility dynamics during chemical induction of pluripotency
            - Kdm2b regulation of somatic reprogramming via variant PRC1 complex
    design:
      columns: '2'

  # Publications
  - block: collection
    id: publications
    content:
      title: Publications
      filters:
        folders:
          - publication
      count: 0
    design:
      columns: '2'
      view: citation

  # Projects
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      buttons:
        - name: All
          tag: '*'
        - name: Single-cell
          tag: scRNA-seq
        - name: Stem Cell
          tag: Stem Cell
    design:
      columns: '1'
      view: showcase

  # Contact
  - block: contact
    id: contact
    content:
      title: Contact
      email: Jian.Wu@innere.med.uni-giessen.de
      phone: '+49 15213499268'
      address:
        street: Aulweg 132
        city: Gießen
        postcode: '35392'
        country: Germany
        country_code: DE
      directions: Center for Infection and Genomics of the Lung (CIGL)
      contact_links:
        - icon: google-scholar
          icon_pack: ai
          name: Google Scholar
          link: 'https://scholar.google.com/citations?user=-pYIKQkAAAAJ&hl'
      autolink: true
    design:
      columns: '2'
---
