# Operational Excellence Primer


## Design Principles

1. Perform operations as code
    * Everything as a source code
    * Compliance, Infrastructure, Delivery Pipeline, Monitoring, Alerting, Playbook

2. Make frequent, small, reversible changes
    * Feature toggles
    * Vertical vs horizontal slicing
    * Trunk-base development
    * Blue green deployments

3. Refine operations procedures frequently
    * Run regular game days
    * Keep the playbook up to date
    * Perform chaos engineering experiments

4. Anticipate failure
    * Perform **pre-mortem** exercises to identify source of failure
    * Murphy's Law - Expecting the Unexpected 
    * Test your failure scenarios and validate impact

5. Learn from all operational failures
    * Run blameless postmortem
    * Create organizational memory
    * Cause and effect analysis - 5 Why's, Fishbone diagram


## How to do

1. Preparation
    - Pre-mortam what could go wrong
    - GamesDay - chaos experiments
        - active failure vs. team tabletops- simulation 
        - fresh understanding 
    - Read and update playbooks

2. Risk Management
    - Frequent, small, reversible changes
    - Feature toggling
    - Blue-green/canary/rolling deployments
    - Bring high-risk items ahead in the project timeline

3. Troubleshooting
    - Triage first
        - make the system work as well as it can under the circumstances
    - Then Examine
        - Each component of the system
        - Metrics plotted as time series
        - Logs - particularly exception and errors
    - Then Diagnose
        - what changed - deployment or config changes
            - See of changes correlating with system bahaviour
        - divide and conquer
            - data flow between components - distributed tracing
            - divide diagnosis by layers or steps
    - Finally test and treat
    - Pitfalls
        - Looking at symptoms that aren’t relevant
        - misunderstanding the meaning of system metric
     
4. Event Response
    - A clear and well-defined line of command
    - Delegated roles and responsibilities
        - Incident commander
        - Response team
        - Communication lead
        - Planning lead
    - Record the state and actions
        - all details of an incident
        - every action on debugging and mitigation

5. Root Cause Analaysis
    - 5 Whys - cause and effect
    - Fishbone diagram 

6. Organizational Learning
    - Creating, retaining, and transferring knowledge within an organization
    - Every problem as an opportunity to build a better organization response
    - Sharing and transparency
        - applied to all systems and teams organization-wide
        - Conduct cross-team reviews of postmortems
        - Postmartems as a source code (linking to improvements)
    - Run blameless postmortems
    - Review postmartems culture
    - Corrective or Preventive Actions


