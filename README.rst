aspects-sample plugin for `Tutor <https://docs.tutor.edly.io>`__
################################################################

aspects-sample plugin for Tutor


Installation
************

.. code-block:: bash

    pip install git+https://github.com/saraburns1/tutor-contrib-aspects-sample
    tutor plugins enable aspects-sample
    tutor config save

Adding New Assets
*****************
Create a dashboard in the Superset UI and export it as a ZIP file.

.. code-block:: bash
    
    tutor aspects import_superset_zip ~/Downloads/your_file.zip --base_assets_path ./tutoraspects_sample/templates/aspects-sample/build/assets

Validate and rebuild:

.. code-block:: bash
    
    tutor aspects check_superset_assets
    tutor local do import-assets


Additional Resources
=====================

- `Superset Documentation <https://superset.apache.org/docs>`_
- `DBT Documentation <https://www.getdbt.com/docs/>`_
- `Clickhouse Documentation <https://clickhouse.com/docs>`_
- `Tutor Documentation <https://docs.tutor.overhang.io>`_
- `Event Routing Backends Documentation <https://event-routing-backends.readthedocs.io/en/latest/>`_
