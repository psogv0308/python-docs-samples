.. This file is automatically generated. Do not edit this file directly.

Google Cloud Speech API Python Samples
===============================================================================

This directory contains samples for Google Cloud Speech API. The `Google Cloud Speech API`_ enables easy integration of Google speech recognition technologies into developer applications. Send audio and receive a text transcription from the Cloud Speech API service.




.. _Google Cloud Speech API: https://cloud.google.com/speech/docs/ 

Setup
-------------------------------------------------------------------------------


Authentication
++++++++++++++

Authentication is typically done through `Application Default Credentials`_,
which means you do not have to change the code to authenticate as long as
your environment has credentials. You have a few options for setting up
authentication:

#. When running locally, use the `Google Cloud SDK`_

    .. code-block:: bash

        gcloud beta auth application-default login


#. When running on App Engine or Compute Engine, credentials are already
   set-up. However, you may need to configure your Compute Engine instance
   with `additional scopes`_.

#. You can create a `Service Account key file`_. This file can be used to
   authenticate to Google Cloud Platform services from any environment. To use
   the file, set the ``GOOGLE_APPLICATION_CREDENTIALS`` environment variable to
   the path to the key file, for example:

    .. code-block:: bash

        export GOOGLE_APPLICATION_CREDENTIALS=/path/to/service_account.json

.. _Application Default Credentials: https://cloud.google.com/docs/authentication#getting_credentials_for_server-centric_flow
.. _additional scopes: https://cloud.google.com/compute/docs/authentication#using
.. _Service Account key file: https://developers.google.com/identity/protocols/OAuth2ServiceAccount#creatinganaccount

Install Dependencies
++++++++++++++++++++

#. Install `pip`_ and `virtualenv`_ if you do not already have them.

#. Create a virtualenv. Samples are compatible with Python 2.7 and 3.4+.

    .. code-block:: bash

        $ virtualenv env
        $ source env/bin/activate

#. Install the dependencies needed to run the samples.

    .. code-block:: bash

        $ pip install -r requirements.txt

.. _pip: https://pip.pypa.io/
.. _virtualenv: https://virtualenv.pypa.io/

Samples
-------------------------------------------------------------------------------

Quickstart
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++



To run this sample:

.. code-block:: bash

    $ python quickstart.py


Transcribe
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++



To run this sample:

.. code-block:: bash

    $ python transcribe.py

    usage: transcribe.py [-h] speech_file
    
    Google Cloud Speech API sample application using the REST API for batch
    processing.
    
    Example usage: python translate.py resources/audio.raw
    
    positional arguments:
      speech_file  Full path of audio file to be recognized
    
    optional arguments:
      -h, --help   show this help message and exit


Transcribe async
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++



To run this sample:

.. code-block:: bash

    $ python transcribe_async.py

    usage: transcribe_async.py [-h] speech_file
    
    Google Cloud Speech API sample application using the REST API for async
    batch processing.
    
    Example usage: python transcribe_async.py resources/audio.raw
    
    positional arguments:
      speech_file  Full path of audio file to be recognized
    
    optional arguments:
      -h, --help   show this help message and exit




The client library
-------------------------------------------------------------------------------

This sample uses the `Google Cloud Client Library for Python`_.
You can read the documentation for more details on API usage and use GitHub
to `browse the source`_ and  `report issues`_.

.. Google Cloud Client Library for Python:
    https://googlecloudplatform.github.io/google-cloud-python/
.. browse the source:
    https://github.com/GoogleCloudPlatform/google-cloud-python
.. report issues:
    https://github.com/GoogleCloudPlatform/google-cloud-python/issues


.. _Google Cloud SDK: https://cloud.google.com/sdk/