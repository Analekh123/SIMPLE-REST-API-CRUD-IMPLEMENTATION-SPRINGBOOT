# SIMPLE-REST-API-CRUD-IMPLEMENTATION-SPRINGBOOT

CloudVendor REST API
This project demonstrates a simple REST API implementation for managing cloud vendor details using Spring Boot. The API supports basic CRUD operations such as creating, retrieving, updating, and deleting cloud vendor data.

Technologies Used
-----------------
Java
Spring Boot
Maven


Endpoints
-----------------------------------------------
The following endpoints are provided by the API:

1. Get Cloud Vendor Details
Endpoint: GET /cloudvendor/{vendorId}
Description: Retrieves the details of a specific cloud vendor.
Parameters:
vendorId (Path Variable): The ID of the cloud vendor to retrieve.
Response:
CloudVendor object with the stored details of the vendor.

Example Request:
GET /cloudvendor/C1

3. Create Cloud Vendor
Endpoint: POST /cloudvendor
Description: Creates a new cloud vendor.
Request Body:
JSON representation of a CloudVendor object.
{
  "vendorId": "C1",
  "vendorName": "Vendor1",
  "vendorAddress": "Address1",
  "vendorPhone": "9946557692"
}
Response:
Success message: "cloud vendor created successfully"
4. Update Cloud Vendor
Endpoint: PUT /cloudvendor
Description: Updates the details of an existing cloud vendor.
Request Body:
JSON representation of the updated CloudVendor object.
Example:
{
  "vendorId": "C1",
  "vendorName": "Updated Vendor",
  "vendorAddress": "Updated Address",
  "vendorPhone": "1234567890"
}
Response:
Success message: "cloud vendor updated successfully"
5. Delete Cloud Vendor
Endpoint: DELETE /cloudvendor/{vendorId}
Description: Deletes a specific cloud vendor.
Parameters:
vendorId (Path Variable): The ID of the cloud vendor to delete.
Response:
Success message: "cloud vendor deleted successfully"

