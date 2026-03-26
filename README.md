# OpenClaw 安装说明（机器人用）

这个技能包只需要复制 2 个文件到 OpenClaw 的 skills 目录。

## 需要复制的文件

1. `SKILL.md`
2. `scripts/polymarket.py`

## 安装步骤

1. 在 OpenClaw 的 skills 目录下新建一个文件夹（例如 `better_polymarket`）。
2. 把本仓库的 `SKILL.md` 复制到该文件夹根目录。
3. 在该文件夹内创建 `scripts/` 子目录。
4. 把本仓库的 `scripts/polymarket.py` 复制到 `scripts/` 目录。

目标结构示例：

```text
<openclaw-skills>/better_polymarket/
  SKILL.md
  scripts/
    polymarket.py
```

## 运行依赖

- 需要 `python3`
- 需要网络访问目标站点的公共 API

## 验证

在机器人环境中执行：

```bash
python3 {baseDir}/scripts/polymarket.py trending
```

如果能正常返回市场数据，说明安装完成。
