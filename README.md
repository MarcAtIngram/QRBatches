This project ingests a specifically formatted .xlsx file and returns a set of QR image files based on the data in the spreadsheet.

Dependencies:
 * openpyxl - reads xlsx files
 * PyQRCode & pypng - writes QR image files

### Using QRBatches:
QRBatches.py: Builds QR codes to link Youtube movie trailers. 
                Writes QR images based on a specifically formatted .xlsx input file 
                        First column is the movie name 
                        Fifth column is the Youtube (longform) link
                        Youtube Asset IDs are 11-character code at the end of the link
                Images generated contain the shortform link (https://youtu.be/[asset ID])
                Images generated are named in "Trailer QR - "[movie name]" - "[Youtube Asset ID]".png" format
