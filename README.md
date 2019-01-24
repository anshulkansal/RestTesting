# Testing using Rest Assured

-Testing and validating REST services in Java is harder than Groovy.
-Rest-Assured begins he simplicity of using these languages into Java domain.

# Using GetWith Parameters:
Public static void performQueryParameter()  {
given()
        .contentTye(COontentType.Json)
        .qyueryParam(s:"id", ...objects:1).
when()
        .get(s:"http://localhost:3000/posts/").
        
then()
        .body(s:"author", hasItem("Karthik kk"));
        }


# Using Path Parameters:

Public static void performPathParamter()  {
given()
        .contentType(Content Type:Json).
with()
        .pathParams(s:"post", o:1)
when()
        .body(s:"author",containsString(subString:"Karthik kk"));
        }

