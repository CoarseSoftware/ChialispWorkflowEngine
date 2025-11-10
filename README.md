# Chialisp Workflow Engine (Early Beta)
### Beta Phase.  Some things may not work, have bugs and be subject to change.  Use the 'Report Bug' button at the bottom of a workflow when your experience is not as expected.
## [chialisp.coarsesoftware.com](https://chialisp.coarsesoftware.com/)

### About
- Chialisp Workflow Engine is used to build and test chialisp puzzles using an intuitive, UX approach.
- 100% Offline - meaning there is no backend or other 3rd party apis.  This ensures puzzles are kept private.
- Logging - logs are used when submitting an issue.  Logs will not track user input data but will contain data about the node hierarchy like puzzle type and puzzle ID.  No logs are sent without the users knowledge.


### Beta -> Release | Roadmap
- chialisp tests
  - wasm for clvm commands using rust clvm tools
- Mimic various chialisp programs
  - ie; https://github.com/Chia-Network/chia-dev-tools/blob/main/cdv/examples/clsp/piggybank.clsp
  - fix any issues along the way
  - find and mimic more advanced puzzles

### Community Participation
Issues, features and feature requests will be tracked using this Github repository.  
- Issues
  - Use the 'Report Bug' view at the bottom of a workflow, which will send the report to Github.

# Tutorial
### Basic Concept
- Starting with a Module node, connect other nodes by dragging a noodle to a desired location and select from a list of child nodes.
### Getting Started
- Select 'New Workflow' from the top right menu, input a name and click create.
### Saving
- press ctrl + s to save your workflow locally.
### Copy/Paste
- copy - highlight nodes, ctrl + c
- paste - ctrl + v
### Open Existing Workflow
- drop a .clwf file.  This will create a new tab for each workflow.
### Testing
- Tests are available at each node.  Open the test tab at the bottom of the node and add a test.  Caution: Tests do require a bit of resources and can greatly reduce performance.  This will be improved on in the future.
### Chialisp
- Select the 'chialisp' tab at the bottom on any node to view/copy the chialisp.

# Special Nodes
## Template Node
- Templates are a way to create re-usable puzzles that can require desired functions and constants as well as requiring user defined nodes to be plugged in.
### Create Template
- Hover over the menu at the bottom of the page and click 'Add Template'.
### Export Template
- Using the menu at the top right of the template node, click 'Export Template'.
### Template Ouput
- Template Output is a selectable node that can be attatched to any child node of a Template.  This will give the user a way to plug in children nodes.
### Using Templates
- Drag out a noodle and then select the 'Pointer -> Template' node.  From there, you can select the template from an exported file or an internal template.  Note: Internal templates do react to changes.

## Chialisp Node
- Node that allows any chialisp to be input.
- Use named inner puzzles to create a connection point to another node.  Anywhere in the chialisp that the name is used, will be replaced with the code generated from the connected node.




