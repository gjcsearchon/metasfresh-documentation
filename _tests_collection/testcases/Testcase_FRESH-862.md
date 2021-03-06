---
title: IT FRESH-862
required data:
   bpartner: bpartner G000X (vendor)
   products: P0001, P0002
   HUs: TU A, TU B
   pricelists: vendor pricelist VP   
layout: default
tags:
  - UI
  - Request
---
## #578 Request Window Attachment Image too large in viewer

> Testcase to check the attachment image in request window.

1. Create requests by creating material receipts with quality issue and quality note, for G000X and P0001 & P0002

1. Open window request (Vorgang alle), click attachment, select a picture from your db, OK
	* => preview of the picture, in a small frame, with scrollbars at the sides
	* => picture is set as attachment, attachment button turns grey

1. Click the attachment button again:
	* => the picture you set as attachment is fully displayed
	* => the OK / Cancel and other buttons can be reached easily, you don't have to move the picture
	
1. Open the other request window (Vorgang), select another entry and repeat (attach another picture):
	* => works the same
	
1. Click attachment again in one of the windows, and add a PDF to the request as well 

1. Open the attachment for this request once more:
	* => picture is displayed first
	* => dropdown at the top, where you can select the pic / the PDF
	* => if the PDF is displayed rather small, you can zoom in with the resp. buttons
	

**Note:** You can change the attached image, in both Vorgang and Vorgang (alle), for the same request; but: if you attach a picture for the first time in one window, and try to attach another picture in the other window without refreshing first, you will get an exception!
