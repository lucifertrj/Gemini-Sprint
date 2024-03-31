# Gemini-Sprint- LlamaIndex and Gemini Examples

## Multimodal RAG

### Input Data

![coimbatore](https://github.com/lucifertrj/Gemini-Sprint/assets/66197713/dd99042d-7a25-4cb4-b368-b79fee72a0e4)

### Data Extracted from LLM

```
{
  "city_name": "Coimbatore",
  "state_name": "Tamil Nadu",
  "famous_food": "South Indian",
  "history": "Coimbatore is a city in the Indian state of Tamil Nadu. It is the second largest city in the state after Chennai. Coimbatore is known for its textile industry and is often referred to as the \"Manchester of South India\". The city is also home to several educational institutions and research centers.",
  "review": "Coimbatore is a beautiful city with a rich history and culture. The city is home to several temples, mosques, and churches. The climate is tropical and the city experiences hot summers and mild winters. The city is well-connected by air, rail, and road. Coimbatore is a major industrial and commercial center and is home to several large corporations. The city is also a major educational center and is home to several universities and colleges.",
  "description": "Coimbatore is a city in the Indian state of Tamil Nadu. It is the second largest city in the state after Chennai. Coimbatore is known for its textile industry and is often referred to as the \"Manchester of South India\". The city is also home to several educational institutions and research centers.",
  "nearby_tourist_places": "Coimbatore is home to several tourist attractions, including the Adiyogi Shiva statue, the Perur Pateeswarar Temple, and the VOC Park and Zoo."
}
```

### Store Information in VectorDB - Qdrant later use it for Q&A

#### User Prompt

```python
response = query_engine.query(
    "which place belongs to Coimbatore from the given context, and tell about that given place history. Also tell whats the best food one can eat there?"
)
print(response)
```

#### LLM Response: 

```bash
The Adiyogi Shiva statue is a 112-foot tall statue of Shiva located in Coimbatore, Tamil Nadu. It is the largest Shiva statue in the world. The statue was consecrated on 24 February 2017 by Sadhguru Jaggi Vasudev, the founder of the Isha Foundation.

The statue is made of concrete and steel and is covered with 500 copper plates. The copper plates were donated by devotees from all over the world. The statue is a symbol of peace and unity and is a popular tourist destination.

The best food to eat in Coimbatore is South Indian food. South Indian food is known for its use of spices and flavors. Some of the most popular South Indian dishes include idli, dosa, vada, and sambar.
```
