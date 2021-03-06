.. _colaboracion:


Colaboración
############


Estructura de la documentación
******************************

La documentación esta estructurada en un árbol de carpetas cuya raíz se divide en "funcional" y en "técnico".

Cada subcarpeta dentro de estas mantiene una organización conceptual agrupando aquellos conceptos que se entienden
dentro de una misma área. Cada concepto tiene su propio archivo .rst dentro de la carpeta donde le corresponda.

Las imágenes se cargan dentro de una carpeta "imagenes" situada en el mismo directorio del .rst que las utiliza.

Cada archivo .rst representa un concepto. Puede tener diferentes apartados, subrayadas con almohadillas, que se pueden dividir
en secciones, subrayadas con asteriscos.


Proceso de Colaboración
***********************

Esta documentación esta supervisada por la Asociación Española de Odoo, pero
confeccionada por la comunidad. Puedes completar, mejorar y corregir la documentación
proponiendo nuevos cambios mediante Github con una Pull Request o una Issue.


Guía de Estilo en Español AEODOO
********************************

La documentación se genera en Español teniendo en cuenta la guía de estilo de traducción al Español (España):

- `Guía de estilo Español <https://www.aeodoo.org/traduccion-de-odoo-al-espanol-de-espana>`_


Edición con ReStructuredText y Sphinx
*************************************

Otro paso a dar para colaborar en la documentación es aprender el lenguaje ReStructuredText y Sphinx.

- ReStructuredText

    - `reStructuredText Primer <https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html>`_

    - `Odoo RST Cheet Sheet <https://www.odoo.com/documentation/user/14.0/contributing/documentation/rst_cheat_sheet.html>`_
    - `Odoo RST Guidelines <https://www.odoo.com/documentation/user/14.0/contributing/documentation/rst_guidelines.html>`_

- Sphinx

   - `Sphinx <https://docs.readthedocs.io/en/stable/intro/getting-started-with-sphinx.html>`_
   - `For Technical Writers <https://www.ericholscher.com/blog/2016/jul/1/sphinx-and-rtd-for-writers/>`_


- Configurar Tema readthedocs

   - `Configurar tema readthedocs <https://sphinx-rtd-theme.readthedocs.io/en/stable/configuring.html>`_


Para generar la documentación tenemos que tener instaladas las dependencias:

.. code-block:: 

    pip install -r source/requirements.txt

Y en el directorio del proyecto clonado de GitHub generamos el código HTML de salida, y comprobamos también los posibles errores con:

.. code-block::

    make html

Para evitar ciertos errores podemos limpiar el directorio de salida y para compilar de nuevo.

.. code-block::

    make clean

    make html