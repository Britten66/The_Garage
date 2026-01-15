# The Garage 

**"Build. Break. Fix."**

Welcome to **The Garage**. This is the central workshop for the reusable tools, hooks, and hardware snippets I use to speed up development and solve recurring problems.

I run a weekly collaborative session called **Coding & Coffee**. I noticed a pattern among the students and juniors attending: we were all rewriting the same boilerplate code over and over again. I built this repo to solve that.
## Features

- **Blueprints (Web & React):** Reusable patterns for modern web development, including custom hooks like `useFetch`.

- **Hardware Lab (IoT & Embedded):** C++ snippets for ESP32/Arduino, including robust WiFi connection logic for unstable environments.

- **Workshop Tools (Java & Scripts):** Utilities born from my SDET background, including timestamped logging and safe File I/O.
## Usage/Examples

The most popular tool in the garage is the `useFetch` hook.

**The Old Way (Boilerplate Way) **
```
useEffect(() => {
  setLoading(true);
  fetch(url)
    .then(res => res.json())
    .then(data => setData(data))
    .catch(err => setError(err))
    .finally(() => setLoading(false));
}, []);

```
## **New Build**
```

const { data, loading, error } = useFetch('[https://api.mysite.com/data](https://api.mysite.com/data)');

```




