# Quick Start Checklist
This is the quick start checklist to get the incident response process working.

## Organizational Preparation
- [ ] Build an asset management
    - use a [template](templates/assetFactsSheet.md)
    - use [tools](examples/assetManagement.md)
- [ ] Define the roles in your incident response team
    - use a [template](templates/rolesAndResponsibilities.md#csirt-roles-template)
    -  minimal needed roles:
        - Incident Investigator
        - Incident Manager
        - Communication Manager 
        - Legal Manager
- [ ] Define roles for each asset / project
    - use a [template](templates/rolesAndResponsibilities.md#project-incident-response-roles-template) 
- [ ] Get contact details for the used cloud providers
- [ ] Get the needed contact for your customer
- [ ] Define access concept
    - how the CSIRT can get read-only access to a cloud environment
    - how the CSIRT can get access in an incident case
    - see [here](preparation/organisational.md#access-concept) on how to build such access concept
    - use a [template](templates/emergencyAccess.md)
- [ ] Define your communication plan
    - to the customer
    - to your cloud provider
    - to the internal organization
    - use some [examples](examples/communication.md)
- [ ] Define the process for incident response
    - use the [example](examples/process.md)
- [ ] Build policies to support the incident response team
    - Incident classification ([See this example](examples/incidentClassification.md))
- [ ] Train the incident response team
    - External trainings
    - Internal trainings
    - War games (See the [examples](examples/warGame.md) and the templates ([This](templates/warGameEvaluation.md) and
    [this](templates/warGamePreparation.md))
    
## Technical preparation
- [ ] Build a central logging concept
    - define the [data sources](examples/dataSources.md)
    - build a central logging solution
    - Analyse your logs with [playbooks](examples/playbooks.md) as support
    - Set up monitoring 
- [ ] Implement the defined access concept
- [ ] Set up a data export concept for infected data (See [here](preparation/technical.md)))
- [ ] Prepare your incident response tool chain with [tools](examples/tools.md)

## Handling an Incident
- [ ] Take care of your input events
- [ ] Classify the event if this is a security related event
- [ ] Triage the event
    - Use [this example](examples/incidentClassification.md) for the classification
- [ ] Start containing the incident
    - Take care of the different cloud service models (See [here](handling/README.md#containment))
- [ ] Recover or rebuild the environment
    - Take care that the evidence won't get deleted
    - Fix the initial attack vector before redeploying
- [ ] Do a root-cause analysis to find all traces from the attacker
    - This helps also to reconstruct what happens and to improve the systems and processes

## Post-Processing
- [ ] Conduct lessons learned
- [ ] Finish the documentation
    - use a [template](templates/incidentFactsSheet.md)
- [ ] Use the gathered knowledge to enhance the organization