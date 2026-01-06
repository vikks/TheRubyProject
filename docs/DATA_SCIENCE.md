# Data Science & Machine Learning in Ruby

While Python is the dominant language for Data Science, Ruby has a growing and highly performant ecosystem that leverages C++ and Rust backends to match industry standards.

## The Ruby Data Stack (vs. Python)

| Python Tool | Ruby Equivalent | Description |
| :--- | :--- | :--- |
| **NumPy** | **[Numo::NArray](https://github.com/ruby-numo/numo-narray)** | Efficient multi-dimensional arrays for Ruby. |
| **Pandas** | **[Polars-ruby](https://github.com/ankane/polars-ruby)** | High-performance DataFrames via Rust Polars. |
| **Pandas (Native)** | **[Rover](https://github.com/ankane/rover)** | Simple, Ruby-idiomatic DataFrames. |
| **Scikit-learn** | **[Rumale](https://github.com/yoshoku/rumale)** | Comprehensive ML library (SVM, Trees, Clustering). |
| **PyTorch** | **[Torch.rb](https://github.com/ankane/torch-rb)** | Ruby bindings for LibTorch (PyTorch C++ backend). |
| **TensorFlow** | **[TensorStream](https://github.com/josephrocca/tensor_stream)** | A ground-up Ruby implementation of TensorFlow. |

## Data Visualization

*   **[Vega-Ruby](https://github.com/ankane/vega):** A high-level grammar of interactive graphics (similar to Altair in Python).
*   **[Nyaplot](https://github.com/SciRuby/nyaplot):** Interactive plots for Ruby notebooks.
*   **[Chartkick](https://chartkick.com/):** Create beautiful JavaScript charts with one line of Ruby.

## Deep Learning & AI

Ruby's approach to deep learning is primarily through **Torch.rb**, which allows you to define models using a syntax nearly identical to Python's PyTorch, but with Ruby's cleaner blocks and method calls.

```ruby
# Example Torch.rb syntax
model = Torch::NN::Sequential.new(
  Torch::NN::Linear.new(20, 64),
  Torch::NN::ReLU.new,
  Torch::NN::Linear.new(64, 10)
)
```

## The "Ankane" Effect
A significant portion of the modern Ruby Data Science ecosystem is maintained by **Andrew Kane (ankane)**, who has systematically ported/built Ruby versions of the most popular Python tools, ensuring Ruby remains viable for data-heavy applications.

## Gaps

*   **Community & Tutorials:** The sheer volume of stack overflow answers and tutorials for Python dwarfs Ruby's data science presence.
*   **Native Integration:** While Ruby has the *libs*, many third-party APIs and SaaS tools only provide Python/JS SDKs for their ML features.
