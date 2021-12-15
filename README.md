# Data Extraction Test

This repo contains the a zip folder with bunch of excel files having sample sale data of different clients and their buyers info(name and pan), puchase amount etc . . .

**Note**:

    Input: 
        filename: consists The name of the clinet, month and year 
        Ex: ALSC_OCT_2021.xlsx 
            ALSC -- client name
            OCT -- month
            2021 -- year
    Output: Output file should contain below mentioned columns.
        pan no:
            PAN number will be unique for each buyer
            Some buyers may provide GST number pan number will be a substring of GST
            Ex:
                GSTNo: 26AADCK8554D1ZI
                    in above gst number AADCK8554D is the pan of buyer.
                Note: A file contains a GST or pan either data we have to store pan number in result file.
            if you didn't pan or GST in put file mark it as N/A in result file
        Turnover:
            Calculate the turnover by aggerating the all transaction ammout made by each buyer for each client.
            Turnover may be in -ve/+ve values.
        client name:
            Get client name from the filename.
        month:
            Get month from the filename.
        Buyer name:
            Get buyer name fron imput file buyer column

**Question**:

    Write a python program to generate the concatinated result file for all 3 inpput files (for input files extract zip file):

