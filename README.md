backend:
  name: git-gateway
  branch: main

media_folder: "assets/images/uploads"
public_folder: "/assets/images/uploads"

collections:
  - name: "pages"
    label: "الصفحات"
    files:
      - file: "content/home.md"
        label: "الرئيسية"
        name: "home"
        fields:
          - { label: "العنوان", name: "title", widget: "string" }
          - { label: "الوصف", name: "description", widget: "text" }

      - file: "content/about.md"
        label: "من نحن"
        name: "about"
        fields:
          - { label: "العنوان", name: "title", widget: "string" }
          - { label: "النص", name: "body", widget: "markdown" }

  - name: "products"
    label: "المنتجات"
    folder: "content/products"
    create: true
    slug: "{{slug}}"
    fields:
      - { label: "اسم المنتج", name: "title", widget: "string" }
      - { label: "الصورة", name: "image", widget: "image" }
      - { label: "الوصف", name: "body", widget: "markdown" }
