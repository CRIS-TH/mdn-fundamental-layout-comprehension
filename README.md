# Fundamental Layout Comprension Tutorial

Follow the [MDN Fundamental Layout Comprension Tutorial](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Fundamental_Layout_Comprehension).

Do the best you can to complete it. Use the **[task hints](#task-hints)** below if needed.

## Starting Point

Download Assets

```bash
# 1. Download `index.html` in your document root directory:
wget https://github.com/mdn/learning-area/raw/main/css/css-layout/fundamental-layout-comprehension/index.html

# 2. And `styles.css`:
wget https://raw.githubusercontent.com/mdn/learning-area/main/css/css-layout/fundamental-layout-comprehension/styles.css

# 3. Make a directory for `images/` and download the five image files:
mkdir images/

## push the current directory on the stack (so we can pop back to it later) and change into it
pushd images/

## download `balloon-sq1.jpg` through `balloon-sq6.jpg` 
for i in {1..6}
do
  wget https://github.com/mdn/learning-area/raw/main/css/css-layout/fundamental-layout-comprehension/images/balloon-sq${i}.jpg
done

## pop the pushed directory off the stack and go back to it
popd

```

### Task Hints

Choose the layout method for steps to follow:

* [Two Column Flexbox Layout](two-col-flexbox-tasks.md)
* [Two Column Grid Layout](two-col-grid-tasks.md)
