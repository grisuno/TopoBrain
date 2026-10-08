# root

*Community 0 | 2 files | cohesion 1.00*

## Definition

This community groups 2 file(s) rooted at `root` with dominant language py (cohesion 1.00). Central symbols: `AdaptiveCombinatorialComplexLayer`, `AsymmetricPredictiveErrorCell`, `CheckpointManager`, `Config`, `ContinuumMemoryCell`, `LearnableAbsenceGating`, `PrefrontalOrchestrator`, `ResidualBlock`. Core file: `app.py` (84 symbols). Documented purpose: Autor: Gris Iscomeback Correo electrónico: grisun0[at]proton[dot]me Fecha de creación: 30/11/2025 Licencia: GPL v3  Descripción:.

## Files

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `app.py` | py | utility | 84 | yes |
| `install.sh` | sh | utility | 0 | no |

## Key Symbols

- `Config` (class, `app.py:41`) `class Config`
- `__post_init__` (method, `app.py:101`) `def __post_init__(self)`
- `to_dict` (method, `app.py:107`) `def to_dict(self)`
- `get_supcon_lambda` (method, `app.py:110`) `def get_supcon_lambda(self, epoch)`
- `get_sparsity_lambda` (method, `app.py:116`) `def get_sparsity_lambda(self, epoch)`
- `seed_everything` (method, `app.py:131`) `def seed_everything(seed)`
- `ResourceMonitor` (class, `app.py:145`) `class ResourceMonitor`
- `get_memory_gb` (method, `app.py:147`) `def get_memory_gb()`
- `get_gpu_memory_gb` (method, `app.py:152`) `def get_gpu_memory_gb()`
- `log` (method, `app.py:158`) `def log(prefix)`
- `clear_cache` (method, `app.py:165`) `def clear_cache()`
- `check_limit` (method, `app.py:171`) `def check_limit(limit_gb, abort_on_limit)`
- `PrefrontalOrchestrator` (class, `app.py:190`) `class PrefrontalOrchestrator(Module)` - Módulo de control ejecutivo que monitoriza el estado de la red y emite señales
- `__init__` (method, `app.py:197`) `def __init__(self, config)`
- `forward` (method, `app.py:234`) `def forward(self, metrics_dict)` - Orquestador v27: Allostasis con Frenado de Emergencia (Gradient-Aware).
- `detach_state` (method, `app.py:334`) `def detach_state(self)` - Rompe el grafo computacional para evitar retropropagación infinita entre batches
- `reset_context` (method, `app.py:339`) `def reset_context(self)` - Resetear contexto al inicio de cada época
- `TopologyMetrics` (class, `app.py:346`) `class TopologyMetrics`
- `TopologicalHealthSovereignty` (class, `app.py:355`) `class TopologicalHealthSovereignty` - Monitor SVD Completo con criterios neurocientíficos
- `__init__` (method, `app.py:362`) `def __init__(self, model, config, epsilon_c)`
- `_analyze_matrix` (method, `app.py:368`) `def _analyze_matrix(self, weight_matrix, name)`
- `calculate` (method, `app.py:414`) `def calculate(self, epoch)`
- `get_critical_summary` (method, `app.py:431`) `def get_critical_summary(self)`
- `CheckpointManager` (class, `app.py:441`) `class CheckpointManager` - Manager robusto v18 con backups y metadata
- `__init__` (method, `app.py:443`) `def __init__(self, run_name)`
- `save` (method, `app.py:448`) `def save(self, data, name)`
- `load` (method, `app.py:476`) `def load(self, name)`
- `get_dataloaders` (method, `app.py:493`) `def get_dataloaders(config)` - DataLoaders con augmentation de alto rendimiento para CIFAR-10
- `SupConLoss` (class, `app.py:537`) `class SupConLoss(Module)`
- `__init__` (method, `app.py:538`) `def __init__(self, temperature)`

## Internal vs External Edges

- Internal resolved imports (EXTRACTED): 0
- Cross-boundary resolved imports (EXTRACTED): 0

## Connections

- No cross-community bridges recorded. This community is self-contained.

## Risks

- No scoped security, taint, cycle, or layer risks.

## Open Questions

- Why do 1 file(s) lack file-level docs (e.g. `install.sh`)? What purpose do they serve?
- What would break if the most connected file in root changed?
- Should root be split, given cohesion 1.00?

## Sources

- `app.py`
- `install.sh`
