# Azure Form Recognizer Demo

<ol>
<li> Setup Azure Portal account following word document</li>
<li> Get API key and endpoint</li>
<li> Add key, endpoint, and PDF URL (any pdf you want to test with) to azure_forms_recognizer_example.py script</li>
<li>run demo</li>

>$ pip install azure-ai-formrecognizer==3.2.0

>$ python azure_forms_recognizer_example.py
</ol>



### Next Steps:
- Detemine need for local container
    - if you need to run locally (at ETSU), who is going to manage the container infrastructure?
    - https://azure.microsoft.com/mediahandler/files/resourcefiles/microsoft-azure-ferpa-implementation-guide/FERPA%20Implementation%20Guide%20for%20Azure.pdf
    - https://learn.microsoft.com/en-us/azure/applied-ai-services/form-recognizer/containers/form-recognizer-container-install-run?view=form-recog-2.1.0&viewFallbackFrom=form-recog-3.0.0&tabs=layout
- Determine storage location for scanned PDFs
   - For example, local or shared drive (:S drive?)
   - if local files:
```
import os

def read_file(file_name):
    file_handle = open(file_name)
    print file_handle.read()
    file_handle.close()
```
- Edit script to send data to RedCap API
    - Create logfile

### References:
- https://github.com/Azure-Samples/cognitive-services-quickstart-code/blob/04742b25209c20321ad4f2bd4e1f3bbf9ea79ae1/python/FormRecognizer/FormRecognizerQuickstart.py#L4
- https://learn.microsoft.com/en-us/python/api/overview/azure/ai-formrecognizer-readme?view=azure-python
- https://learn.microsoft.com/en-us/azure/applied-ai-services/form-recognizer/quickstarts/get-started-sdks-rest-api?view=form-recog-3.0.0&pivots=programming-language-python
- 
