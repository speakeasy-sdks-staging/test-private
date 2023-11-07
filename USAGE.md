<!-- Start SDK Example Usage -->


```go
package main

import (
	"context"
	testprivate "github.com/speakeasy-sdks-staging/test-private"
	"log"
)

func main() {
	s := testprivate.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx)
	if err != nil {
		log.Fatal(err)
	}

	if res.StatusCode == http.StatusOK {
		// handle response
	}
}

```
<!-- End SDK Example Usage -->