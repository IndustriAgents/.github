# IndustriAgents

**Open-source tools that connect AI agents to industrial machines.**

We build tools for developers working at the intersection of industrial automation and AI. Our projects connect agents to machine data through industrial protocols and the Model Context Protocol (MCP).

[Explore public repositories](https://github.com/orgs/IndustriAgents/repositories?type=public) · [Visit our website](https://www.industriagents.com/)

## Start with a project

| Project | Start here if you work with |
| --- | --- |
| [OPCUA-MCP](https://github.com/IndustriAgents/OPCUA-MCP) | OPC UA servers and machine data |
| [MQTT-MCP](https://github.com/IndustriAgents/MQTT-MCP) | MQTT brokers and connected devices |

Open the project README for setup instructions and examples.

## Get involved

- **Report a bug.** Open an issue in the relevant repository with your version, what you expected, and steps to reproduce it.
- **Propose an integration.** Describe the protocol, device, or workflow you want to support and what a working example would look like.
- **Contribute.** Documentation fixes, examples, tests, and code are welcome. For larger changes, open an issue first to discuss the scope.

See each repository for its license and contribution guidance.
# IndustriAgents

**Connect AI agents to your machines.**

IndustriAgents builds open-source tools that give AI agents access to industrial equipment, the documentation to understand what they observe, and explicit limits on what they can do. The projects bring together industrial automation, the Model Context Protocol (MCP), and evidence-backed knowledge graphs.

[Website](https://industriagents.com/) · [Try a simulated machine](https://industriagents.com/connect#setup) · [Explore public repositories](https://github.com/orgs/IndustriAgents/repositories?type=public)

| Layer | What it does | Where to start |
| --- | --- | --- |
| **Connect** | Read live data from PLCs, SCADA systems, and IIoT brokers through local MCP servers. | [IndustriConnect](https://github.com/IndustriAgents/IndustriConnect) |
| **Context** | Turn manuals, specifications, and procedures into reviewed knowledge graphs with source evidence. | [OntoLab](https://github.com/IndustriAgents/OntoLab) |
| **Control** | Start read-only and scope any enabled writes with policy and per-server audit records. | [Control documentation](https://industriagents.com/control) |

## Connect · Industrial protocols over MCP

[IndustriConnect](https://github.com/IndustriAgents/IndustriConnect) brings together ten protocol servers, simulated devices, and a web console. Use one server with your MCP client, or explore several protocols in one place. [IndustriCode](https://github.com/IndustriAgents/IndustriCode) is a separate chat interface that connects MCP tools to cloud or local models.

<details>
<summary><strong>Browse the ten protocol servers</strong></summary>

| Protocol | Repository | Typical use |
| --- | --- | --- |
| OPC UA | [OPCUA-MCP](https://github.com/IndustriAgents/OPCUA-MCP) | Browse nodes, read live values and history, and follow subscriptions and alarms |
| Modbus | [MODBUS-MCP](https://github.com/IndustriAgents/MODBUS-MCP) | Work with registers and coils over TCP, UDP, or serial RTU |
| Siemens S7 | [S7comm-MCP](https://github.com/IndustriAgents/S7comm-MCP) | Read Siemens PLC data blocks, I/O, markers, and CPU state |
| EtherNet/IP | [EtherNetIP-MCP](https://github.com/IndustriAgents/EtherNetIP-MCP) | Browse and read Allen-Bradley Logix tags |
| MQTT / Sparkplug B | [MQTT-MCP](https://github.com/IndustriAgents/MQTT-MCP) | Subscribe to broker topics and decode Sparkplug B payloads |
| BACnet/IP | [BACnet-MCP](https://github.com/IndustriAgents/BACnet-MCP) | Discover building automation devices and read object properties |
| DNP3 | [DNP3-MCP](https://github.com/IndustriAgents/DNP3-MCP) | Read SCADA outstation points and run class polls over TCP |
| EtherCAT | [EtherCAT-MCP](https://github.com/IndustriAgents/EtherCAT-MCP) | Scan EtherCAT segments and inspect process data and CoE objects |
| PROFINET | [PROFINET-MCP](https://github.com/IndustriAgents/PROFINET-MCP) | Discover devices and inspect GSDML descriptions |
| PROFIBUS DP | [PROFIBUS-MCP](https://github.com/IndustriAgents/PROFIBUS-MCP) | Explore cyclic I/O and diagnostics with a mock slave |

</details>

Live equipment support varies by protocol. EtherCAT requires dedicated network access, and PROFINET and PROFIBUS DP have preview backends. See the [protocol support matrix](https://industriagents.com/connect) for hardware and testing status.

## Context · Knowledge grounded in source documents

A live value can tell an agent that an input is on. A knowledge graph can identify the sensor, show which station it belongs to, and point to the relevant passage in the manual.

| Project | What it does |
| --- | --- |
| [OntoLab](https://github.com/IndustriAgents/OntoLab) | Build or import an ontology, extract facts with source passages, review and validate them, and export RDF. |
| [OntoLab Desktop](https://github.com/IndustriAgents/OntoLab-Desktop) | Try the document-to-graph workflow on an Apple silicon Mac with the desktop preview. |
| [GraphMind](https://industriagents.com/context) | Explore a graph visually and ask questions about it in the invite-only web preview. |
| [FB2Skill](https://github.com/IndustriAgents/FB2Skill) | Convert IEC 61499 function blocks into RDF skill descriptions using MAESTRO or CaSkMan. |

## Control · Explicit permissions for machine actions

**Available today.** Protocol servers start read-only. Writes require explicit enablement. Server policies can restrict operations and record write intent before a command is sent. Start with a bundled simulator when evaluating an agent workflow.

**In development.** A shared policy gateway, dry runs and approval for proposed writes, and a cross-server audit log. Follow the [Control layer](https://industriagents.com/control) for the current status.

## Contribute

Open an issue in the relevant repository for a protocol gap, a reproducible bug, or a feature proposal. Simulator scenarios, protocol fixtures, setup examples, and documentation improvements are welcome. For a larger change, open an issue to discuss the scope before submitting a pull request.

See each repository for its license and contribution guidance. For pilots, systems integration, or research collaboration, reach us at [hi@industriagents.com](mailto:hi@industriagents.com).

## Contact

For general inquiries, email [hi@industriagents.com](mailto:hi@industriagents.com).
