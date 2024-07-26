# PIC-with-4-level-priority-resolver-for-multicore-processor

# Overview
This project implements a programmable interrupt controller designed for a quad-core processor. It features dynamic priority assignment for interrupt requests and supports parallel servicing of interrupts for each core. The controller ensures high-priority requests are served first while handling up to four interrupt requests per core simultaneously.

# Features
- # Dynamic Priority Assignment:
- Interrupt priorities can be assigned and adjusted dynamically, providing flexible interrupt management.
- # Parallel Request Servicing:
- Capable of handling four interrupt requests simultaneously with four interrupt request lines to four cores of CPU.
- # Priority Resolver:
- Resolves interrupt requests based on their priority levels to ensure the highest priority interrupt is selected for servicing.
- # Masking of Request:
- Any unwanted interrupt can be masked by wirting into Masked_irr register.

# Components
- # Interrupt Request Lines (IRQ):
- Total 32 interrupt lines for 32 peripheral devices.Each having a priority levels.
- # Interrupt Service Register (ISR):
- Stores addresses of service routines for each interrupt type, allowing quick and efficient response to interrupts.
- # Vector Address:
- Sends the vector address of the interrupt that is currently being served to the particular core through data bus.
