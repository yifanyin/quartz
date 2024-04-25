---
title: "Basic models of seismicity: Spatiotemporal models"
tags:
  - reference
DocumentClass:
  - report
authors:
  - "[[Jiancang Zhuang]]"
  - "[[Maximilian Jonas Werner]]"
  - "[[Sebastian Hainzl]]"
  - "[[David S Harte]]"
  - Shiyong Zhou
source:
  - CORSSA
---
# Basic models of seismicity : Spatiotemporal models
- Authors: [[Jiancang Zhuang]], [[Maximilian Jonas Werner]], [[Sebastian Hainzl]], [[David S Harte]], Shiyong Zhou
- Date: 2011
- Source: the Community Online Resource for Statistical Seismicity Analysis
- Links:: [[statistical seismology]]

## Abstract
In this article, we present a review of spatiotemporal point-process models, including the Epidemic-Type Aftershocks Sequence ([[ETAS]]) model, the EEPAS (Every Earthquake is Precursor According to Scale) model, the double branching model, and related techniques. Here we emphasize the ETAS model, because it has been well studied and is currently a standard model for testing hypotheses related to seismic activity.

## Notes
The temporal form of ETAS model shown as the conditional intensity function

$$\lambda(t)=\mu+\displaystyle K_0\sum_{t_i<t}\frac{\exp(\alpha(m-m_0))}{(t-t_i+c)p} \tag{1}$$ 

$\mu$ is the background rate, $K_0$ is the productivity of an event. c and p are parameters in the [[Statistical seismology#Omori-Utsu law|Omori-Utsu law]]

Spatial-temporal form from [[Ogata.AnnInstStatMath.1998]]

$$\lambda(t, x, y, m)=s(m)[\mu(x,y)+\displaystyle\sum_{k: t_k<t} \kappa(m_k)g(t_k)f(x-x_k, y-y_k; m_k)] \tag{10}$$

$\mu(x,y)$ is the background intensity function, which is assumed to be independent of time. The functions $g(t), f(x,y;m_k)$ and s(m) are respectively the normalized response functions (i.e., probability density functions) of the occurrence time, the location, the magnitude of an offspring from an ancestor of magnitude $m_k$.

We note that $\kappa(m_k)$ is the expected number of children from a parent of size $m_k$

$$s(m)=\beta e^{-\beta(m-m_0)}$$
