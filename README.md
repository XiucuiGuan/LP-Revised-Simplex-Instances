# LP-Revised-Simplex-Instances
You can generate random LP instances with 4 variables and 2 constraints, in which x3 and x4 are the initial basis variables. Then choose an entering variable and leaving variable, run the revised simplex algorithm to solve it.

# 修正单纯形法演示程序

本项目实现了一个修正单纯形法的演示程序，用于求解线性规划问题。修正单纯形法通过维护基逆矩阵（B⁻¹）来提高计算效率，特别适用于大规模线性规划问题，但是本演示程序只提供小规模例子的迭代过程，帮助初学者理解算法，还有问题没有修复，仅用来演示简单的迭代。

## 文件说明

### `revisedsimplex_kimi.txt`
- **功能**：实现了一个修正单纯形法的演示程序。
- **特点**：
  - 支持随机生成线性规划问题实例。
  - 提供中间计算表格，展示基逆矩阵、入基列、右端列等关键信息。
  - 支持手动输入入基和出基变量进行迭代。
  - 在达到最优解时，显示最终结果并提示用户。

## 使用说明

1. **生成新问题**：
   - 点击“生成新问题”按钮，程序将随机生成一个新的线性规划问题实例。

2. **确定入基变量**：
   - 查看初始单纯形表，确定入基变量（负检验数对应的列）。
   - 在输入框中输入入基变量（如 `x1`、`x2` 等），然后点击“生成中间表格”按钮。

3. **确定出基变量**：
   - 根据最小比值规则确定出基变量。
   - 在输入框中输入出基变量（如 `x3`、`x4` 等），然后点击“执行迭代”按钮。

4. **观察迭代过程**：
   - 程序将展示迭代后的修正单纯形表，包括基逆矩阵、当前解、检验数和目标函数值。

5. **最优解判断**：
   - 如果所有检验数非负，程序将提示已达到最优解。

## 运行方式

1. 将 `revisedsimplex_kimi.txt` 文件下载到本地。
2. 使用浏览器打开文件即可运行程序。

## 依赖

- 本程序为纯 HTML 和 JavaScript 实现，无需额外依赖。

## 贡献

欢迎提交 Issue 或 Pull Request 来改进代码或文档。

## 许可证

本项目采用 [MIT 许可证](LICENSE)。
