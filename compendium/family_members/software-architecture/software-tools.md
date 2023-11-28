# Software Tools

The OEFamily provides several small software tools for specific tasks.

## OEP-Client

The client is a well-developed command line interface (CLI) that can be used to interact with the OEP and in particular with the OEDB database. It offers functions for uploading and downloading data and metadata from the local file storage and is considered the most important CLI tool for all technical users who want to get started quickly.

!!! info "Access oep-client"
    <https://github.com/OpenEnergyPlatform/oep-client>

## omi - Open Metadata Integration

The Open Metadata Integration OMI tool is used for programmatic work with the [oemetadata](../templates-and-specification/open-energy-metadata.md) specification. It can be used for technical operations such as parsing, compiling, rendering, converting and validating the JSON-based metadata specification. It is integrated into the Open Energy Platform and takes responsibility for parsing all metadata before it is stored in a table.

!!! Warning
    The tool is still in use, but is also considered oversized as it takes on too many responsibilities and requires more maintenance effort than expected. We are currently looking into a new implementation.

!!! info "Access omi"
    <https://github.com/OpenEnergyPlatform/omi>

## saio - SQLAlchemy Input/Output

SQLAchemy input output is a small software module for the Python library SQLAlchemy. It enables the automated generation of database table objects in python code. For this purpose, the table structure on the OEDB is used and automatically translated into an ORM. This simplifies object-oriented interaction with the database. However, this module does not have a special user interface and should be integrated into other software.

!!! info "Access saio"
    <https://github.com/OpenEnergyPlatform/saio>

## oem2orm - Open Energy Metadata to Object Relational Mapper

Open Energy Metadata to ORM is a great tool that can be used to automatically create one or more tables on the OEDB database from the Open Energy Metadata Json files. As indicated, it is assumed that metadata already exists in the oemetadata format and that the resources in particular are filled in there. The resources are a key in the JSON document in which the structure of the table is stored schematically.

!!! info "Access oem2orm"
    <https://github.com/OpenEnergyPlatform/oem2orm>

## oedialect- Open Energy Dialect

The Open Energy Dialect is a tool that provides a so-called database dialect specifically for the OEDB. It uses the Python library SQLAlchemy, which can interpret these dialects to gain access to the OEDB via the REST-API of the Open Energy Platform and, for example, to upload and download data there. The oedialect also does not provide its own user interface and should be integrated into other software. 

!!! Warning
    The oedialect is still used, but works with a very old version of SQLAlchemy and needs a revision or update. it is mainly used for the so-called extended api of the OEP, which enables extensive database access, but is rarely used by public users, as it is mainly used for other software tools that require this extensive access.

!!! info "Access the oedialect"
    <https://github.com/OpenEnergyPlatform/oedialect>
