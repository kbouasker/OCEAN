OCEAN Documentation
===================

**Open-source CXL Emulation at Hyperscale Architecture and Networking**

Welcome to the OCEAN documentation.

OCEAN is an open-source emulation framework for researching and experimenting with
Compute Express Link (CXL)–based memory systems. It provides a software environment
to explore memory disaggregation, pooling, and multi-host access in the absence of
widely available production CXL hardware.

What is OCEAN?
--------------

OCEAN (Open-source CXL Emulation at Hyperscale Architecture and Networking) enables
system-level experimentation with CXL-inspired architectures by emulating key
components of CXL fabrics and memory devices.

As CXL standards continue to evolve, OCEAN is designed to support research,
prototyping, and evaluation of memory system designs, software stacks, and
application behavior in disaggregated and pooled memory environments.

Why OCEAN?
----------
CXL 3.0 introduces transformative memory pooling and fabric management capabilities,
but the lack of available hardware poses significant barriers to research. Existing
emulation approaches focus on single-host scenarios or lack CXL 3.0 features, limiting
their utility for datacenter-scale research.

**OCEAN addresses this gap by providing:**

* **Multi-host memory pooling** — Memory sharing across multiple virtual machines 
  for realistic datacenter scenarios
* **CXL 3.0 compliance** — Full protocol support including fabric management, 
  dynamic capacity devices, and configurable switch topologies
* **Full-system emulation** — Runs unmodified production workloads without 
  application changes
* **Performance fidelity** — Achieves emulation within approximately 3x of 
  projected native CXL speeds
* **Research flexibility** — Configurable topology, policies, and instrumentation

OCEAN is intended to support:

* **Research and Prototyping**  
  Explore CXL-based memory architectures and system designs in a controlled,
  software-based environment.

* **System-Level Evaluation**  
  Study how operating systems and applications interact with shared and pooled
  memory resources.

* **Architecture Exploration**  
  Investigate design trade-offs in memory disaggregation, fabric topologies, and
  resource management policies.

* **Software Development**  
  Develop and test software for CXL-like memory systems without requiring physical
  CXL hardware.

Key Capabilities
----------------

OCEAN provides:

* Emulation of CXL-based memory fabrics and device topologies
* Support for multi-host access to shared and pooled memory
* Dynamic allocation and management of memory resources
* Integration with existing software stacks for experimentation
* Ability to run real workloads to study system behavior

Use Cases
---------

Current use cases supported by OCEAN include:

* Evaluation of memory pooling across multiple hosts
* Exploration of shared memory access patterns in disaggregated systems
* Prototyping and testing of CXL-aware system software and applications

Quick Start
-----------

.. code-block:: bash

   git clone https://github.com/cxl-emu/OCEAN.git
   cd OCEAN
   bash ./script/setup_host.sh
   bash ./script/setup_network.sh 2

For more details, see :doc:`getting-started`.

Documentation Structure
-----------------------

This documentation is organized into the following sections:

* :doc:`getting-started` — Installation and first experiments
* :doc:`architecture` — Overview of OCEAN's architecture and components
* :doc:`configuration` — Configuration and customization options
* :doc:`workloads` — Workloads and experiments with CXL memory

.. toctree::
   :maxdepth: 1
   :hidden:
   
   getting-started
   architecture
   configuration
   workloads

Community
---------

* **Project Website**: https://cxl-emu.github.io
* **GitHub Repository**: https://github.com/cxl-emu/OCEAN
