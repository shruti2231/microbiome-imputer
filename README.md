# Microbiome Imputer

**Microbiome Imputer** is a Python package for imputing missing values in microbiome abundance data using a denoising autoencoder model. It helps researchers and bioinformaticians clean and preprocess their microbiome datasets efficiently.

---

## Features

- Imputes missing or zero values in microbiome abundance profiles
- Uses pretrained Denoising Autoencoder models for better accuracy
- Easy command-line interface for quick imputation
- Handles input and output in CSV format

---

## Installation

Install the package via PyPI:

```bash
pip install microbiome-imputer
```

## Usage

After installation, you can use the `microbiome-imputer` command-line tool to impute your microbiome data.

```bash
microbiome-imputer  
```

* `<input_csv>`: Path to your input CSV file containing microbiome abundance data.
* `<output_csv>`: Path where the imputed output CSV file will be saved.

Example:

```bash
microbiome-imputer sp_profile.csv imputed.csv
```

This command will load the input file `sp_profile.csv`, perform imputation, and save the imputed data as `imputed.csv`.

## Input File Format

* The input CSV should contain species abundance profiles.
* Ensure the data is numeric and missing values or zeros represent data points to be imputed.
* The last three columns can be categorical and will be preserved without modification.

## Notes

* The package includes pretrained models and necessary JSON files internally.
* TensorFlow is required and will output some logs on first run.
* For large datasets, the process might take some time depending on your system specs.

## Development

To clone the repository and install in development mode:

```bash
git clone https://github.com/shruti2231/microbiome-imputer.git
cd microbiome-imputer
pip install -e .
```

## License

This project is licensed under the MIT License.

## Contact

For any questions or issues, please open an issue on GitHub or contact the maintainer.

**Happy imputing!**