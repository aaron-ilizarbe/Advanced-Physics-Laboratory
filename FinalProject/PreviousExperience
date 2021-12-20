#!/usr/bin/env python
# coding: utf-8

# # Frecuencia Fundamental de la copa de vidrio.

# In[1]:


from numpy import*
from pylab import plot, grid, xlabel, ylabel, title, show, xlim
cupgru = loadtxt("Prueba11.txt", float)


# ### A partir del aplicativo Phyphox obtenemos los datos de Amplitud y Tiempo, graficamos Amplitud vs Tiempo. 
# La amplitud está en u.a(Unidades adimensionales) y el tiempo en segundos.

# In[2]:


plot(cupgru[:,0], cupgru[:,1])
grid()
title("Oscilaciones de la copa")
ylabel("Amplitud(a.u))")
xlabel("t(s)")
show()


# ### Graficamos las oscilaciones entre los segundos 0 y 0.0355 para observar mejor el comportamiento del periodo.

# In[3]:


plot(cupgru[:,0], cupgru[:,1])
xlim(0,0.00355)
grid()
ylabel(r"$Amplitud(a.u)$")
title("Oscilaciones entre los segundos [0, 0.00355]")
show()


# ### Análisis FFT realizado por el aplicativo Phyphox

# In[4]:


picos = loadtxt("Prueba11picosfreq.txt", float)


# In[5]:


plot(picos[:,0], picos[:,1])
grid()
#xlim(0, 5100)
title("Picos de frecuencia")
ylabel("Amplitud(u.a))")
xlabel("Frecuencia(Hz)")
show()


# In[6]:


# Definimos fm como la mayor amplitud entre las frecuencias.
fm = max(picos[:,1])
fm


# In[7]:


# Calculamos la frecuencia asociada a esta amplitud.
print ("El elemento de array con la frecuencia de mayor amplitud es:", where(picos[:,1]==30.80246464) )
# Y la imprimimos
print("La frecuencia fundamental de la copa es:", picos[338,0], "Hz")


# In[ ]:




