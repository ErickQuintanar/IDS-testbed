# Change Management

The change management process focuses on four pillars: understanding the change to be made, planning this change, implementing the change, and communicating the change. There can be several reasons for the need to change the Testbed, such as, a new component version, changes in the component requirements that the environment or the component must meet, and changes in the Information Model. This document will cover the process in detail to successfully proceed to include changes into the Testbed.

## Including a new component or an existing component’s new version into the Testbed

The Testbed will serve as the environment where collaborators can work on the interoperability between components within the IDSA environment. The Testbed with the validated components and their respective versions will be available in the following Github repository (https://github.com/International-Data-Spaces-Association/IDS-testbed/tree/master/Testbed).

The following procedure will be followed for the inclusion of new components and/or component versions for the different components in the Testbed.

The new component and/or component version will be isolated with respect to the Testbed directory. The component’s code quality, documentation and functionality will be evaluated. Every modification and/or new feature(s) with respect to previous versions, if any, must be clearly documented.

Once the modification and/or new feature(s) have been verified, interoperability will be tested in a trial Testbed. Here, the component will be slowly connected to the other components to ensure that functionality remains as expected until the trial Testbed includes every previously included component. 

The list of points that are checked:
•	Documentation must be complete (installation manual, user manual, etc.)
•	Security profile requirements of the component are fulfilled
•	Code quality
•	Operational procedures
•	Interoperability functionality

Basic example: New Dataspace Connector version. The connector will be placed in a new isolation directory. This directory will be the trial Testbed area for the new component versions. The connector’s code, documentation and functionality will be checked. The Dataspace Connector will act as both provider and consumer while isolated. Once the functionality works as intended, the connector will be connected to DAPS. Once these connect as expected, the Broker will be added to the environment and verify that the connection is possible.

If the new component and/or component version successfully interacts with the trial Testbed, it is ready to be moved into the Testbed.

The updates that occur in the Testbed must be included in an update log where the changes, dates, and team in charge of validation will be detailed.

If a new component and/or component version demands changes in the installation and/or interoperability document of the Testbed, the new documents must be available and reference the Testbed version they apply to.

## Criterion changes/updates

Components affected by the changes directly (affects component’s funcionality/security) or indirectly (require extra features to accept new funcionality/security from other components) should be notified. The components will have to upgrade their components to meet the new requirements and go through the “Including a new component or an existing component’s new version into the Testbed” section of this document.

Important: If major criterion changes were to occur that may cause those non-updated components to disrupt the expected behavior of the IDSA architecture, the Testbed maintainers may be able to disable/remove such components temporarily.

## Changes in the Information Model

The TestBed environment and the validated components will have an identifier associated with the version of the Information Model to which it applies.

When significant changes in the IDS Information Model occur, they will be clearly reflected in the Information Model’s Github repository.  

The release process will always be aligned with the IDSA architecture, and the new validated Information Model for the TestBed will be indicated in the corresponding release of the TestBed.