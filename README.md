# **JPSS Data Explorer**

This project provides a simple, browser-based tool to explore and access satellite imagery data collected from the Joint Polar Satellite System (JPSS) instruments (NOAA-20, NOAA-21, and SNPP). It facilitates quick discovery of NetCDF4 files stored in public AWS S3 buckets.

There is a version hosted via github pages at [https://coliveir-aer.github.io/jpss-data-explorer/](https://coliveir-aer.github.io/jpss-data-explorer/)

## **Key Features**

* **Satellite Selection:** Choose between NOAA-20, NOAA-21, and SNPP satellites.  
* **Instrument and Product Selection:** Select from various instruments (e.g., VIIRS, ATMS, CrIS, OMPS) and their associated data products using a hierarchical filtering system.  
* **Date/Time Filtering:** Specify a particular date and time window to narrow down search results.  
* **S3 Bucket Exploration:** The application queries specific S3 bucket paths to list available files for the selected criteria.  
* **File Download:** Directly download HDF5/NetCDF4 data files from the S3 bucket.  
* **Easy File Viewing:** Open selected HDF5 files directly in myhdf5.hdfgroup.org for immediate viewing.  
* **Product Information:** Displays a mapping of JPSS product display names to their corresponding S3 directory names.

## **How to Use**

1. **Clone this repository:**  
   git clone https://github.com/coliveir-aer/jpss-data-explorer.git  
   cd jpss-data-explorer

2. Open index.html:  
   To utilize all features, host index.html on a web server (e.g., GitHub Pages) or open it directly in your browser.

## **Data Source**

This explorer accesses public JPSS data directly from AWS S3 buckets, ensuring broad accessibility and ease of use.

## **Technologies Used**

* **HTML5:** For the web page structure.  
* **CSS3 (Tailwind CSS):** For responsive and modern styling.  
* **JavaScript (Frontend Vanilla JS):** Handles client-side logic and interaction with the AWS S3 (ListObjectsV2) API.  
* **AWS S3 Public Datasets:** The source of JPSS satellite data.
