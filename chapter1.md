---
title: 'Chapter Title Here'
description: 'Chapter description goes here.'
---

## Example coding exercise

```yaml
type: NormalExercise
key: 2bafef99a3
lang: r
xp: 100
skills: 1
```

This is an example exercise.

`@instructions`


`@hint`


`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}

```

`@solution`
```{r}

```

`@sct`
```{r}

```

---

## Insert exercise title here

```yaml
type: NormalExercise
key: 5eaed185a3
xp: 100
```



`@instructions`
Fit a linear model to the gala dataset

`@hint`


`@pre_exercise_code`
```{r}
require(faraway)
```

`@sample_code`
```{r}

```

`@solution`
```{r}
lm.fit <- lm(Species ~ Area + Elevation + Nearest + Scruz + Adjacent, 
            data = gala)
coef <- lm.fit$coefficients
```

`@sct`
```{r}
ex() %>% check_object(.,"coef") %>% check_equal() 

```
