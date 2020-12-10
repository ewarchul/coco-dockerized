## Installation 

### Requirements

* Docker (version 19.03.13)
* docker-compose (version 1.27.4)
* Python (version 2.7)

Last requirement means that your algorithm should be executable in `Python 2.7`.

Clone this repository and run below command:

```
docker-compose build
```

## Usage

### Run benchmark

Read `experiment.py` documentation and modify that file according to your goals. 

To run benchmark suite for your favorite algorithm execute written below command:

```
docker-compose up coco_executor
```

Application will save benchmark results to `exdata` directory. Don't forget to check if you have permission to read that directory.

### Results processing

Modify `post-processing.sh` script and run below command:

```
docker-compose up coco_plotter
```

Application will create `ppdata` directory which contains processed benchmark(s) results. 

It will also create `index.html` file which is a convenient way to look through obtained results.
