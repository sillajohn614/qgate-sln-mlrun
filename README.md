# QGate-Sln-MLRun
Quality Gate for solution MLRun (and Iguazio). The main aims of the project are:
- independent quality test (function, integration, acceptance, ... tests)
- deeper quality checks before rollout to company environments
- identification of compatibility issues
- external test coverage
- etc.

The tests use these key components:
 - MLRun solution (used in Iguazio solution also), see **[GIT mlrun](https://github.com/mlrun/mlrun)**
 - Sample data model, see **[GIT qgate-model](https://github.com/george0st/qgate-model)**

## Usage
You can easy use this solution in three steps:
1. Download content of these two GIT repositories to your local environment
    - [qgate-sln-mlrun](https://github.com/george0st/qgate-sln-mlrun)
    - [qgate-model](https://github.com/george0st/qgate-model)
2. Update file `qgate-sln-mlrun.env` from qgate-model
   - Update variables for MLRun/Iguazio, see `MLRUN_DBPATH`, `V3IO_USERNAME`, `V3IO_ACCESS_KEY`, `V3IO_API`
     - setting of `V3IO_*` is needed only in case of Iguazio installation (not for pure/free MLRun)
   - Update variables for QGate, see `qgate-model`
3. Run from QGate-MLRun
   - **python main.py**

Precondition: You have available MLRun (tested with >= 1.3.0) or Iguazio solution (MLRun is part of that), see [installation steps](https://docs.mlrun.org/en/latest/install.html)

## Use cases
Quality Gate covers these use cases, TBD.