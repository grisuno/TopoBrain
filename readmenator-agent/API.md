# API

## app.py

### seed_everything `def seed_everything(seed)`
- Defined: `app.py:131`

### get_dataloaders `def get_dataloaders(config)`
- Defined: `app.py:493`
- Doc: DataLoaders con augmentation de alto rendimiento para CIFAR-10

### save_topology_visualization `def save_topology_visualization(model, epoch, run_name)`
- Defined: `app.py:1418`
- Doc: Visualización v18 completa

### save_node_importance_viz `def save_node_importance_viz(model, epoch, run_name)`
- Defined: `app.py:1462`
- Doc: Visualización de importancia de nodos v18

### analyze_topology_clustering `def analyze_topology_clustering(model, run_name)`
- Defined: `app.py:1484`
- Doc: Clustering espectral v18

### analyze_topology_flow `def analyze_topology_flow(model, dataloader, run_name, num_samples)`
- Defined: `app.py:1523`
- Doc: Análisis de flujo de información con captura genérica de outputs

### visualize_topology_as_graph `def visualize_topology_as_graph(model, run_name, threshold)`
- Defined: `app.py:1589`
- Doc: Grafo v18 con métricas

### analyze_topology_evolution `def analyze_topology_evolution(run_name)`
- Defined: `app.py:1641`
- Doc: Análisis temporal completo v18

### comprehensive_topology_analysis `def comprehensive_topology_analysis(model, dataloader, run_name)`
- Defined: `app.py:1702`
- Doc: Suite completa de análisis v18

### run_ablation_study `def run_ablation_study()`
- Defined: `app.py:1725`
- Doc: Suite de ablación v18 completa

### visualize_memory_evolution `def visualize_memory_evolution(model, epoch, run_name)`
- Defined: `app.py:1826`
- Doc: Visualiza evolución de memorias semánticas

### analyze_gradient_flow `def analyze_gradient_flow(model, epoch, run_name)`
- Defined: `app.py:1917`
- Doc: Análisis detallado del flujo de gradientes

### make_adversarial_pgd `def make_adversarial_pgd(model, x, y, eps, steps, dataset_name, controls, prev_states)`
- Defined: `app.py:1984`
- Doc: PGD ataque con congelamiento total de pesos y detach explícito de estados.

### evaluate `def evaluate(model, loader, config, adversarial, controls)`
- Defined: `app.py:2062`
- Doc: Evaluación con plasticidad residual (test-time adaptation)

### train_epoch `def train_epoch(model, loader, optimizer, opt_topo, config, epoch, monitor, scaler, sparsity_lambda)`
- Defined: `app.py:2134`
- Doc: Entrenamiento homeostático con lista manual en lugar de deque

### train_model `def train_model(config, run_name)`
- Defined: `app.py:2359`

### main `def main()`
- Defined: `app.py:2530`
- Doc: CLI v24 completo con Orquestador Prefrontal

### __post_init__ `def __post_init__(self)`
- Defined: `app.py:101`

### to_dict `def to_dict(self)`
- Defined: `app.py:107`

### get_supcon_lambda `def get_supcon_lambda(self, epoch)`
- Defined: `app.py:110`

### get_sparsity_lambda `def get_sparsity_lambda(self, epoch)`
- Defined: `app.py:116`

### get_memory_gb `def get_memory_gb()`
- Defined: `app.py:147`

### get_gpu_memory_gb `def get_gpu_memory_gb()`
- Defined: `app.py:152`

### log `def log(prefix)`
- Defined: `app.py:158`

### clear_cache `def clear_cache()`
- Defined: `app.py:165`

### check_limit `def check_limit(limit_gb, abort_on_limit)`
- Defined: `app.py:171`

### __init__ `def __init__(self, config)`
- Defined: `app.py:197`

### forward `def forward(self, metrics_dict)`
- Defined: `app.py:234`
- Doc: Orquestador v27: Allostasis con Frenado de Emergencia (Gradient-Aware).

### detach_state `def detach_state(self)`
- Defined: `app.py:334`
- Doc: Rompe el grafo computacional para evitar retropropagación infinita entre batches

### reset_context `def reset_context(self)`
- Defined: `app.py:339`
- Doc: Resetear contexto al inicio de cada época

### __init__ `def __init__(self, model, config, epsilon_c)`
- Defined: `app.py:362`

### _analyze_matrix `def _analyze_matrix(self, weight_matrix, name)`
- Defined: `app.py:368`

### calculate `def calculate(self, epoch)`
- Defined: `app.py:414`

### get_critical_summary `def get_critical_summary(self)`
- Defined: `app.py:431`

### __init__ `def __init__(self, run_name)`
- Defined: `app.py:443`

### save `def save(self, data, name)`
- Defined: `app.py:448`

### load `def load(self, name)`
- Defined: `app.py:476`

### __init__ `def __init__(self, temperature)`
- Defined: `app.py:538`

### forward `def forward(self, features, labels)`
- Defined: `app.py:541`

### __init__ `def __init__(self, dim, use_spectral)`
- Defined: `app.py:555`

### forward `def forward(self, input_signal, prediction)`
- Defined: `app.py:565`

### __init__ `def __init__(self, dim, min_gate)`
- Defined: `app.py:575`

### forward `def forward(self, x_sensory, x_prediction)`
- Defined: `app.py:585`

### __init__ `def __init__(self, dim, num_atoms)`
- Defined: `app.py:593`

### _maintain_orthogonality `def _maintain_orthogonality(self)`
- Defined: `app.py:607`

### forward `def forward(self, x)`
- Defined: `app.py:612`

### __init__ `def __init__(self, input_dim, hidden_dim, fast_lr, forget_rate, use_spectral)`
- Defined: `app.py:638`

### forward `def forward(self, x, state_M, controls)`
- Defined: `app.py:687`

### __init__ `def __init__(self, in_dim, hid_dim, num_nodes, config, layer_type, layer_idx)`
- Defined: `app.py:763`

### invalidate_sparse_cache `def invalidate_sparse_cache(self)`
- Defined: `app.py:801`

### _validate_and_fix_state `def _validate_and_fix_state(self, state, expected_shape, batch_size, device, state_name)`
- Defined: `app.py:804`

### get_node_importance `def get_node_importance(self)`
- Defined: `app.py:823`
- Doc: FIX: Método faltante para obtener importancia de nodos

### forward `def forward(self, x_nodes, adjacency, incidence, adj_sparse, inc_sparse, prev_state_node, prev_state_cell, controls)`
- Defined: `app.py:829`
- Doc: Forward con señales de control del Orquestador y retorno de ortho deviation

### __init__ `def __init__(self, in_channels, out_channels, stride)`
- Defined: `app.py:959`

### forward `def forward(self, x)`
- Defined: `app.py:973`

### __init__ `def __init__(self, output_dim, grid_size)`
- Defined: `app.py:980`

### forward `def forward(self, x)`
- Defined: `app.py:1006`

### __init__ `def __init__(self, config, in_channels)`
- Defined: `app.py:1035`

### initialize_memories `def initialize_memories(self, dataloader)`
- Defined: `app.py:1099`

### _initialize_layer_memory `def _initialize_layer_memory(self, cell, x_input, name)`
- Defined: `app.py:1136`

### consolidate_semantic_memories `def consolidate_semantic_memories(self)`
- Defined: `app.py:1153`

### set_epoch `def set_epoch(self, epoch)`
- Defined: `app.py:1181`

### calculate_ortho_loss `def calculate_ortho_loss(self, ortho_deviation, controls)`
- Defined: `app.py:1186`

### calculate_topology_diversity_loss `def calculate_topology_diversity_loss(self, controls)`
- Defined: `app.py:1192`

### _init_grid_topology `def _init_grid_topology(self, N)`
- Defined: `app.py:1205`

### get_topology `def get_topology(self, return_sparse)`
- Defined: `app.py:1227`

### forward `def forward(self, x, prev_states, controls)`
- Defined: `app.py:1238`

### prune_topology `def prune_topology(self, controls)`
- Defined: `app.py:1310`

### warmup_topo `def warmup_topo(epoch)`
- Defined: `app.py:2393`
