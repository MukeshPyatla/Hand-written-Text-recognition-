# Hand-written-Text-recognition-
By using python based on transformer model

The free demo of the original TrOCR can be used via API

  Use the gradio_client Python library to query the demo via API.

 -> pip install gradio_client

 After installing library then fetch the interface through api for demo.

  from gradio_client import Client

client = Client("https://nielsr-trocr-handwritten.hf.space/")
result = client.predict(
				"https://raw.githubusercontent.com/gradio-app/gradio/main/test/test_files/bus.png",	# str representing filepath or URL to image in 'image' Image component
				api_name="/predict"
)
print(result)
