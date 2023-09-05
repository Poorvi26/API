Rijksmuseum API automation in Postman - 

Created a Collection which includes the following folders - 

Collection API - GET /api/[culture]/collection
Collection Details API - GET /api/[culture]/collection/[object-number]
Collection Image API - GET /api/[culture]/collection/[object-number]/tiles

1.Collection API - GET /api/[culture]/collection has following request with test cases in it 

Verify Valid Key cases

Test cases - 
 1.Test Case 1: Verify for Valid Key
2.Test Case 2: Verify response contains data
3.Test Case 3: Verify response format is json
4.Test Case 4: Verify the principalOrFirstMaker Name in the Response
5.Test Case 5: Verify the name in the Response
6.Test Case 6: Verify the objectnumber in the Response
7.Test Case 7: Verify the id in the Response

 Verify Invalid Key cases
  
Test Case 8: Verify for an Invalid API Key

Verify type of format

Test Case 9: Verify the response format is XML


2. Collection Details API - GET /api/[culture]/collection/[object-number]


Verify Valid key and Objectnumber


Test cases - 
Test Case 1: Verify for an Valid Key and objectnumber
Test Case 2: Verify format is json
 Test Case 3: Verify the title in the Response
Test Case 4: Verify the objectnumber in the Response
Test Case 5: Verify the id in the Response
Test Case 6: Verify the language nl in the Response


Verify Invalid key


             Test Case 7: Verify invalid key in the Response


Verify Invalid objectnumber


                Test Case 8: Verify invalid objectnumber in the Response
      
Verify Format type as XML
     
                Test Case 9: Verify XML format in the Response


 Verify language as en


                Test Case 10 : Verify the language en in the Response








3. Collection Image API - GET /api/[culture]/collection/[object-number]/tiles

Verify Valid key and object number 

       
                      Test cases - 

                       Test Case 1: Verify for Valid Key status code
                       Test Case 2: Verify specific title in the Response
                       Test Case 3: Verify specific width in the Response
                       Test Case 4: Verify specific height in the Response
                      Test Case 5: Verify specific value of x in the Response
                      Test Case 6: Verify specific value of y in the Response
                      Test Case 5: Verify specific value of url in the Response


Issues found - 


Test Case 8: Verify invalid objectnumber in the Response - 


When providing objectnumber as invalid example 876787
Expected - Error should be displayed indicating object number is invalid
Actual - 500 Internal server error 




Test Case 10 : Verify the language en in the Response
When providing language parameter value as en
Expected - Response should be successful and response language should be en
Actual - Language value is returned as nl 










     



















 

