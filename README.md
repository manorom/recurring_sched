# recurring_sched

Simple scheduling of recurring jobs in Python: Providing a simple, human
readable syntax for recurring jobs and Python's
[sched](https://docs.python.org/3/library/sched.html) module.

Heavily inspired by (the much more feature complete) [scheduler](https://github.com/dbader/schedule).

## Usage

```bash
$ pip install recurring_sched
```

```python
from recurring_sched import RecurringScheduler
def job(message="General Kenobi"):
    print("Hello There: ", message)

schedule.every(10).minutes.do(job)
schedule.every(1).hours.at("30:00").do(job, messages="General Skywalker")
schedule.run()

```
