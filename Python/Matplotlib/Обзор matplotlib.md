**Matplotlib** - мультиплатформенная библиотека для построения и отображения графиков, основанная на массивах библиотеки *NumPy* и спроектированная в расчете на работу с обширным стеком *SciPy*.

Чтобы установить **matplotlib** используется следующая команда:
```bash
pip install matplotlib
```

Чтобы импортировать библиотеку используется следующую строчки кода
```python
import matplotlib as mpl # mpl - общепринятый псевдоним
import matplotlib.pyplot as plt # plt - общепринятый псевдоним
```

Для отрисовки графиков **matplotlib** может использовать в качестве бэкенда следующие библиотеки:
- **Qt5Agg** - рендеринг графики в Qt5 (*требуется PyQt5*). В IPython активируется командой `%matplotlib qt5`
- **ipympl** - рендеринг графики в виджете Jupyter (*требуется ipympl*). В IPython активируется командой `%matplotlib ipympl`
- **GTK3Agg** - рендеринг графики в GTK 3.x (*требуется PyGObject и pycairo или cairocffi*). В IPython активируется командой `%matplotlib gtk3`
- **macosx** - рендеринг графики в Cocoa. В IPython активируется командой `%matplotlib osx`
- **TkAgg** - рендеринг графики в Tk (требуется Tkinter). В IPython активируется командой `%matplotlib tk`
- **nbAgg** - рендеринг графики в Jupyter notebook. В Jupyter активируется командой `%matplotlib notebook`
- **WebAgg** - для использования с торнадо-сервером
- **GTK3Cairo** - Cairo рендеринг графики в GTK 3.x.x (*требуется PyGObject и pycairo или cairocffi*)
- **Qt4Agg** - рендеринг графики в Qt4 (*требуется PyQt4 или pyside*). В IPython активируется командой `%matplotlib qt4`
- **wxAgg** - рендеринг графики в wxWidgets (*требуется wxPython 4*). В IPython активируется командой `matplotlib wx`

Для смены бэкенда **matplotlib** используется команда - `matplotlib.use()`. Например:
```python
import matplotlib

matplotlib.use('Qt5Agg')
print(matplotlib.get_backend()) # Для получения текущего бэкенда
```

Читать далее [[Как отображать графики]].