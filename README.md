<h4 align="center">📦 The Olivia Kit for Golang</h4>

## How to use it
Here is a code example to see how to use the Go kit.
```golang
var information map[string]interface{}
client, err := NewClient("localhost:8080", true, &information)
if err != nil {
	panic(err)
}

defer client.Close()

client.SendMessage("Hello Olivia!")
```