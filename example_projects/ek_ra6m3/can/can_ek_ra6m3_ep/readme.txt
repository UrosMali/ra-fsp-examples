/***********************************************************************************************************************
* 
* Copyright [2020] Renesas Electronics Corporation and/or its affiliates.  All Rights Reserved.
*
* This software is supplied by Renesas Electronics America Inc. and may only be used with products of Renesas Electronics Corp.
* and its affiliates (“Renesas”).  No other uses are authorized.  This software is protected under all applicable laws, 
* including copyright laws.
* Renesas reserves the right to change or discontinue this software.
* THE SOFTWARE IS DELIVERED TO YOU “AS IS,” AND RENESAS MAKES NO REPRESENTATIONS OR WARRANTIES, AND TO THE FULLEST EXTENT 
* PERMISSIBLE UNDER APPLICABLE LAW,DISCLAIMS ALL WARRANTIES, WHETHER EXPLICITLY OR IMPLICITLY, INCLUDING WARRANTIES OF 
* MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, AND NONINFRINGEMENT, WITH RESPECT TO THE SOFTWARE.  TO THE MAXIMUM 
* EXTENT PERMITTED BY LAW, IN NO EVENT WILL RENESAS BE LIABLE TO YOU IN CONNECTION WITH THE SOFTWARE (OR ANY PERSON 
* OR ENTITY CLAIMING RIGHTS DERIVED FROM YOU) FOR ANY LOSS, DAMAGES, OR CLAIMS WHATSOEVER, INCLUDING, WITHOUT LIMITATION, 
* ANY DIRECT, CONSEQUENTIAL, SPECIAL, INDIRECT, PUNITIVE, OR INCIDENTAL DAMAGES;
* ANY LOST PROFITS, OTHER ECONOMIC DAMAGE, PROPERTY DAMAGE, OR PERSONAL INJURY; AND EVEN IF RENESAS HAS BEEN ADVISED OF 
* THE POSSIBILITY OF SUCH LOSS,DAMAGES, CLAIMS OR COSTS.
* 
**********************************************************************************************************************/

1. Project Overview:
       This project demonstrates the basic functionality of CAN running on Renesas RA MCUs using 2 RA boards. On pressing 
       the user button on Board1, data is transmitted to Board2. On receiving the data,  Board2 displays the data on RTTViewer.
       On successful comparison of data, Board 2 transmits the framed data to Board1 as received acknowledgment. Also, whenever 
       the transmission is completed, status is printed on the RTTViewer.


2. Hardware Connections:
       Require 2 CAN transceiver boards (Part# Waveshare SN65HVD230) and 2 RA boards to run the project

       Supported RA Boards: ek-ra6m1, ek-ra6m2, ek-ra6m3, ek-ra6m3g
        
        CAN Transceiver Board1:
	   CANL:Transceiver Board 2 (CANL)
           CANH:Transceiver Board 2 (CANH)
	   CTX: P-401 (RA Board 1)
	   CRX: P-402 (RA Board 1)
	   3.3V: Vcc (RA Board 1)
	   GND: Vss/GND (RA Board 1)

        CAN Transceiver Board2:
	   CANL:Transceiver Board 1 (CANL)
	   CANH:Transceiver Board 1 (CANH)	 
	   CTX: P-401 (RA Board 2)
	   CRX: P-402 (RA Board 2)
	   3.3V: Vcc (RA Board 2)
	   GND: Vss/GND (RA Board 2)