# Scenario Bundles

The Scenario Bundles provide a interface to store and present dedicated information about specific scenarios for which projection data is available on the OEP.
They are based on the concepts available in the [Open Energy Ontology](../knowledge-representation/oeo.md) (OEO)
and the [Open Energy Knowledge Graph](../knowledge-representation/oekg.md) (OEKG).
This enables the OEP to include information on the scenario projection
data available in the database, the corresponding frameworks and models applied (available as [factsheets](factsheets.md) on the OEP),and the study context.

In detail we specify scenario bundles as:

[Scenario bundles](http://openenergyplatform.org/ontology/oeo/OEO_00020227) weave together important information about one or more [scenarios](http://openenergyplatform.org/ontology/oeo/OEO_00000364). They inform about [studies](http://openenergyplatform.org/ontology/oeo/OEO_00020011) made based on a scenario, including publications (= [study report](http://openenergyplatform.org/ontology/oeo/OEO_00020012)).

If there is quantitative [input data](http://openenergyplatform.org/ontology/oeo/OEO_00030029) and / or [output data](http://openenergy-platform.org/ontology/oeo/OEO_00020013) available on the OEP, the scenario bundles can link to that data, too. They can also inform about [models](http://openenergyplatform.org/ontology/oeo/OEO_00020353) (if available as a [model factsheet](https://openenergyplatform.org/factsheets/models/)) and frameworks (if available as a [framework factsheet](https://openenergyplatform.org/factsheets/frameworks/)) that were used to project a scenario into the future (= [scenario projection](http://openenergyplatform.org/ontology/oeo/OEO_00010262)).

In a nutshell: A scenario bundle provides you with all relevant information to understand a scenario's context and to ease a potential re-use of quantitative data for your purposes.

!!! info "Access the Scenario Bundles"
    [openenergyplatform.org/scenario-bundles/main](https://openenergy-platform.org/scenario-bundles/main)

## Scenario Bundles on the OpenEnergyPlatform

The main page displays a list of bundles created by various users and organizations. Users can select a bundle to view it in detail or click the scenario badges to start a qualitative comparison.

<figure markdown>
  ![Image title](../../img/Bundles_main_page.png)
  <figcaption>List of bundles</figcaption>
</figure>

Bundles can be accessed in two modes: view mode, which allows users to see the bundles. The edit mode enables users to make changes to the bundles.

<figure markdown>
  ![Image title](../../img/Bundles_View_Mode.png)
  <figcaption>View a bundle</figcaption>
</figure>

<figure markdown>
  ![Image title](../../img/Bundles_Edit_Mode.png)
  <figcaption>Edit a bundle and add scenarios</figcaption>
</figure>

The comparison show scenarios from different bundles next to each other and displays similarities and differences for comparison.

<figure markdown>
  ![Image title](../../img/Bundles_Qualititative_Comparison.png)
  <figcaption>An example of a qualititative comparison between bundles</figcaption>
</figure>
