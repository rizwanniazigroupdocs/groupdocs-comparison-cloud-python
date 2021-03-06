# GroupDocs.Comparison Cloud Python SDK
Python package for communicating with the GroupDocs.Comparison Cloud API

## Requirements

Python 2.7 or 3.4+

## Installation
Install `groupdocs-comparison-cloud` with [PIP](https://pypi.org/project/pip/) from [PyPI](https://pypi.org/) by:

```sh
pip install groupdocs-comparison-cloud
```

Or clone repository and install it via [Setuptools](http://pypi.python.org/pypi/setuptools): 

```sh
python setup.py install
```

## Getting Started

Please follow the [installation procedure](#installation) and then run following:

```python
# Import module
import groupdocs_comparison_cloud

# Get your app_sid and app_key at https://dashboard.groupdocs.cloud (free registration is required).
app_sid = "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
app_key = "XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"

# Create instance of the API
api = groupdocs_comparison_cloud.InfoApi.from_keys(app_sid, app_key)

try:
    # Retrieve supported file-formats
    response = api.get_supported_file_formats()

    # Print out supported file-formats
    print("Supported file-formats:")
    for format in response.formats:
        print('{0} ({1})'.format(format.file_format, format.extension)) 
except groupdocs_comparison_cloud.ApiException as e:
    print("Exception when calling get_supported_file_formats: {0}".format(e.message))
```

## Licensing
GroupDocs.Comparison Cloud Python SDK licensed under [MIT License](http://github.com/groupdocs-comparison-cloud/groupdocs-comparison-cloud-python/LICENSE).

## Resources
+ [**Website**](https://www.groupdocs.cloud)
+ [**Product Home**](https://products.groupdocs.cloud/comparison)
+ [**Documentation**](https://docs.groupdocs.cloud/comparison)
+ [**Free Support Forum**](https://forum.groupdocs.cloud/c/comparison)
+ [**Blog**](https://blog.groupdocs.cloud/category/comparison)

## Contact Us
Your feedback is very important to us. Please feel free to contact us using our [Support Forums](https://forum.groupdocs.cloud/c/comparison).