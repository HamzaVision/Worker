# Real-time Dashboard

## Description

This project is a real-time dashboard that fetches data from  'https://jsonplaceholder.typicode.com/todos' API and allows users to filter the data based on a provided input. The application demonstrates two filtering methods: one without using a Web Worker and the other using a Web Worker. The goal is to compare the performance of both methods and understand the benefits provided by using Web Workers.

## Instructions to Run Locally

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/real-time-dashboard.git
   ```


2. Open the project folder:

   ```bash
   cd real-time-dashboard
   ```

3. Open the `index.html` file in your web browser.

4. Enter a filter value in the input field to see the filtered data and the time taken for both methods.

## Summary of Performance Findings

The application allows users to compare the time required to filter data with and without using a Web Worker. In some cases, it may be observed that the Web Worker takes more time than without it. This could be due to various factors, such as the small size of the dataset, network latency, and the asynchronous nature of Web Workers. Generally, Web Workers are more beneficial for computationally expensive tasks or when dealing with large datasets.

## Challenges Faced and Solutions

One challenge faced during the development was the observation that Web Workers took more time in some scenarios. To address this, it's crucial to consider factors such as task complexity, data size, and network latency when deciding whether to use a Web Worker. Additionally, proper profiling and testing are essential to identify the most suitable approach for a specific use case.

## Resources

- [MDN Web Docs: Web Workers](https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API)
- [Web Workers Basics - web.dev](https://web.dev/articles/workers-basics)

