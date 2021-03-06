# react-goodreads-shelf

This React component allows you to display a public Goodreads shelf in a React application. It's a lot like the Goodreads JavaScript widget, but allows for more customization, better async loading, and React-like usage.

## Installation

```
npm install --save react-goodreads-shelf
```
or
```
yarn add react-goodreads-shelf
```

## Usage

```jsx
import React from "react";
import { GoodreadsBookshelf } from "react-goodreads-shelf";

function App() {
	return (
		<GoodreadsBookshelf userId="USER_ID_HERE" apiKey="API_KEY_HERE" />
	);
}

export default App;
```

## Customization

You can also set some options as supported by the Goodreads API:

| Option | Type | Description | Default |
| ------ | ---- | ----------- | ------- |
| shelf  | string | The shelf from which to fetch books | read
| sort  | string | The order in which to sort the results returned | date_read
| limit  | number | The maximum number of books to be returned | 10
| width | number | Minimum width allowed for each book | 100
| details | boolean | Whether to show book details like book title, author, and summary | false

## ToDo

Short-term plans include adding additional API options and styling