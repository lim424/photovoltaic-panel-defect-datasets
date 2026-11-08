# Photovoltaic Panel Defect Detection Datasets

This repository contains two YOLO-format datasets for photovoltaic panel defect detection:

- `infrared/`: infrared images with the classes `diode` and `hotspot`.
- `visible/`: visible-light images with the classes `faulty` and `no faulty`.

## Directory layout

Each dataset keeps the standard YOLO split layout:

```text
<dataset>/
  train/images/
  train/labels/
  valid/images/
  valid/labels/
  test/images/
  test/labels/
  data.yaml
```

The corresponding `data.yaml` file can be passed directly to a YOLO training pipeline from inside its dataset directory.

## Dataset details

| Dataset | Files | Classes | Format |
| --- | ---: | --- | --- |
| Infrared | 1,871 | `diode`, `hotspot` | YOLO detection |
| Visible light | 4,201 | `faulty`, `no faulty` | YOLO detection |

The infrared dataset was originally exported from the Roboflow project [solar-panel-infrared-images](https://universe.roboflow.com/solarpanelimages/solar-panel-infrared-images) and is attributed under CC BY 4.0. The repository owner confirms that the visible-light dataset may also be distributed under CC BY 4.0.

## Data availability

This repository currently contains only a subset of the data used in the study. The complete dataset contains 1,200 self-collected images together with two publicly available datasets, totaling 6,000 paired images. The full dataset will be released after the associated paper is published.

## License

Unless a file states otherwise, the datasets and accompanying documentation are released under the [Creative Commons Attribution 4.0 International license](LICENSE). Please retain attribution when redistributing or reusing the data.
