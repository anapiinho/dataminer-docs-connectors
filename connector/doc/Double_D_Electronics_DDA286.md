---
uid: Connector_help_Double_D_Electronics_DDA286
---

# Double D Electronics DDA286

The DDA286 is a family of units and modules for switching controllers (including LNA/LNB controllers) and switching systems where a network port is desirable

## About

This connector monitors the activity of **DDA286** Networkable Switching Controller using a serial connection.

### Version Info

| Range                | Description                                     | DCF Integration     | Cassandra Compliant |
|----------------------|------------------------------------------------ |---------------------|-------------------------|
| 2.0.0.x              | Initial Version                                 | No                  | False                   |
| 2.0.1.x              |                                                 | No                  | False                   |
| 2.0.2.x [SLC Main]   | Fixed discreets issue on Switch lock parameters | No                  | False                   |
                        
### Product Info

| Range | Supported Firmware Version |
|------------------|-----------------------------|
| 2.0.0.x          | Unknown                     |
| 2.0.1.x          | Unknown                     |
| 2.0.2.x          | Unknown                     |

## Installation and configuration

### Creation

#### Serial Main Connection

This connector uses a serial connection and requires the following input during element creation:

SERIAL CONNECTION:

- Direct connection:
  - **Baudrate**: Baudrate specified in the manual of the device.
  - **Databits**: Databits specified in the manual of the device.
  - **Stopbits**: Stopbits specified in the manual of the device.
  - **Parity**: Parity specified in the manual of the device.
  - **FlowControl**: FlowControl specified in the manual of the device.
- Interface connection:
  - **IP address/host**: The polling IP of the device.
  - **IP port**: The IP port of the device.
  - **Bus address**: The bus address of the device.

## Usage

### General

This page displays information about the **Software Version**, the **Device Name**, the **Highest Numbered Switch Supported**

On this page, you can define the **Control Mode** (*Remote* or *Local*) and the **Global Device Mode** (*Auto* or *Manual*).

In addition, you can also view the state of the **Alarms** and there is a button to **Acknowledge** the alarms.

### Regular Switches

This page displays information about the **Position**, the **Locked** state and the **Fault** of the different regular switches of the device.

The page also allows you to change the **Position** of the regular switches.

On the subpage **Route Calculation**, you can upload a CSV file to change the switch paths. The CSV file should use the following format:

```
IP Address 1;IP Address 2
IP Address X;IP Address Y
```

### Multi-Position Switches

This page displays information about the **Position**, the **Locked** state and the **Fault** of the different Multi-Position switches of the device.

The page also allows you to change the **Position** of the Multi-Position switches.

### Alarms

This page displays **HPA** Alarms.
