# Comparing `tmp/PeakDetective-0.1.6.tar.gz` & `tmp/PeakDetective-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PeakDetective-0.1.6.tar", last modified: Wed Apr 19 20:20:05 2023, max compression
+gzip compressed data, was "PeakDetective-0.1.8.tar", last modified: Mon Jul 31 13:44:50 2023, max compression
```

## Comparing `PeakDetective-0.1.6.tar` & `PeakDetective-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/
--rw-rw-rw-   0        0        0      712 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/PeakDetective/
--rw-rw-rw-   0        0        0    45471 2023-04-06 17:44:24.000000 PeakDetective-0.1.6/PeakDetective/__init__.py
--rw-rw-rw-   0        0        0    11229 2023-03-21 22:15:29.000000 PeakDetective-0.1.6/PeakDetective/detection_helper.py
--rw-rw-rw-   0        0        0     1715 2023-01-30 16:28:13.000000 PeakDetective-0.1.6/PeakDetective/find_peaks.R
--rw-rw-rw-   0        0        0      340 2023-01-29 14:48:51.000000 PeakDetective-0.1.6/PeakDetective/install_R_packages.R
--rw-rw-rw-   0        0        0     1978 2023-01-19 22:58:22.000000 PeakDetective-0.1.6/PeakDetective/mz_unity.R
-drwxrwxrwx   0        0        0        0 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/PeakDetective.egg-info/
--rw-rw-rw-   0        0        0      712 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/PeakDetective.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/PeakDetective.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/PeakDetective.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/PeakDetective.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/PeakDetective.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1771 2023-04-19 20:14:53.000000 PeakDetective-0.1.6/setup.py
+drwxr-xr-x   0 ethanstancliffe   (501) staff       (20)        0 2023-07-31 13:44:50.564110 PeakDetective-0.1.8/
+-rw-r--r--   0 ethanstancliffe   (501) staff       (20)     1069 2023-03-29 13:41:03.000000 PeakDetective-0.1.8/LICENSE.txt
+-rw-r--r--   0 ethanstancliffe   (501) staff       (20)      682 2023-07-31 13:44:50.564011 PeakDetective-0.1.8/PKG-INFO
+drwxr-xr-x   0 ethanstancliffe   (501) staff       (20)        0 2023-07-31 13:44:50.563350 PeakDetective-0.1.8/PeakDetective/
+-rw-r--r--   0 ethanstancliffe   (501) staff       (20)    48112 2023-07-11 02:08:39.000000 PeakDetective-0.1.8/PeakDetective/__init__.py
+-rw-r--r--   0 ethanstancliffe   (501) staff       (20)    10950 2023-03-29 13:41:03.000000 PeakDetective-0.1.8/PeakDetective/detection_helper.py
+-rw-r--r--   0 ethanstancliffe   (501) staff       (20)     1647 2023-03-29 13:41:03.000000 PeakDetective-0.1.8/PeakDetective/find_peaks.R
+-rw-r--r--   0 ethanstancliffe   (501) staff       (20)      331 2023-03-29 13:41:03.000000 PeakDetective-0.1.8/PeakDetective/install_R_packages.R
+-rw-r--r--   0 ethanstancliffe   (501) staff       (20)     1886 2023-03-29 13:41:03.000000 PeakDetective-0.1.8/PeakDetective/mz_unity.R
+drwxr-xr-x   0 ethanstancliffe   (501) staff       (20)        0 2023-07-31 13:44:50.563870 PeakDetective-0.1.8/PeakDetective.egg-info/
+-rw-r--r--   0 ethanstancliffe   (501) staff       (20)      682 2023-07-31 13:44:50.000000 PeakDetective-0.1.8/PeakDetective.egg-info/PKG-INFO
+-rw-r--r--   0 ethanstancliffe   (501) staff       (20)      351 2023-07-31 13:44:50.000000 PeakDetective-0.1.8/PeakDetective.egg-info/SOURCES.txt
+-rw-r--r--   0 ethanstancliffe   (501) staff       (20)        1 2023-07-31 13:44:50.000000 PeakDetective-0.1.8/PeakDetective.egg-info/dependency_links.txt
+-rw-r--r--   0 ethanstancliffe   (501) staff       (20)       65 2023-07-31 13:44:50.000000 PeakDetective-0.1.8/PeakDetective.egg-info/requires.txt
+-rw-r--r--   0 ethanstancliffe   (501) staff       (20)       14 2023-07-31 13:44:50.000000 PeakDetective-0.1.8/PeakDetective.egg-info/top_level.txt
+-rw-r--r--   0 ethanstancliffe   (501) staff       (20)       38 2023-07-31 13:44:50.564142 PeakDetective-0.1.8/setup.cfg
+-rw-r--r--   0 ethanstancliffe   (501) staff       (20)     1738 2023-07-31 13:35:32.000000 PeakDetective-0.1.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PeakDetective-0.1.6/PeakDetective/__init__.py` & `PeakDetective-0.1.8/PeakDetective/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1238 +1,1323 @@
-from pyteomics import mzml
-import sys
-import numpy as np
-import matplotlib.pyplot as plt
-from multiprocessing import Manager,Pool
-from threading import Thread
-from tensorflow import keras
-from keras.constraints import max_norm
-import keras.layers as layers
-import scipy.stats as stats
-from bisect import bisect_left
-import math
-import random as rd
-import IPython.display
-from copy import deepcopy
-import pandas as pd
-from scipy.spatial.distance import euclidean
-from fastdtw import fastdtw
-from scipy.interpolate import interp1d
-import pickle as pkl
-import os
-import sklearn.metrics as met
-import datetime
-
-
-class PeakDetective():
-    """
-    Class for curation/detection of LC/MS peaks in untargeted metabolomics data
-    """
-    def __init__(self,resolution=60,numCores=1,windowSize = 1.0):
-        """
-        Constructor for PeakDetective object
-        @param resolution: int, number of datapoints to sample in the EIC window
-        @param numCores: int, number of processor cores to use for concurrent computations
-        @param windowSize: float, size of EIC window to extract (in minutes)
-        """
-        self.resolution = resolution
-        self.numCores = numCores
-        self.windowSize = windowSize
-        self.smoother = Smoother(resolution)
-        self.classifier = ClassifierLatent(5)
-        self.encoder = keras.Model(self.smoother.input, self.smoother.layers[7].output)
-
-    def save(self,path):
-        """
-        Save model weights to given path
-        @param path: str, path where weights should be saved
-        @return: None
-        """
-        if not os.path.exists(path): os.mkdir(path)
-        pkl.dump([self.resolution,self.windowSize],open(path+"parameters.pd","wb"))
-        self.smoother.save(path + "smoother.h5")
-        self.classifier.save(path+"classifier.h5")
-        self.encoder.save(path+"encoder.h5")
-
-
-    def load(self,path):
-        """
-        Load model weights
-        @param path: str, path to folder where model weights were saved
-        @return: None
-        """
-        try:
-            [self.resouton,self.windowSize] = pkl.load(open(path + "parameters.pd","rb"))
-            self.smoother = keras.models.load_model(path+"smoother.h5")
-            self.classifier = keras.models.load_model(path+"classifier.h5")
-            self.encoder = keras.models.load_model(path+"encoder.h5")
-
-        except:
-            print("Error: pd and h5 files were not found, check path")
-
-    def plot_overlayedEIC(self,rawdatas,mz,rt_start,rt_end,alpha=0.3):
-        """
-        Plot an overlayed EIC for specified samples and mz and retention time range
-        @param rawdatas: list of rawData objects, samples to plot EIC for
-        @param mz: float, m/z value to extract EIC
-        @param rt_start: float, retention time value that is the starting value to plot
-        @param rt_end: float, retention time value that is the ending value to plot
-        @param alpha: float, transparency factor (0-1)
-        @return: None
-        """
-        ts = np.linspace(rt_start,rt_end,self.resolution)
-        for data in rawdatas:
-            s = data.interpolate_data(mz,rt_start,rt_end)
-            ints  = [np.max([x,0]) for x in s(ts)]
-            plt.plot(ts,ints,alpha=alpha)
-
-
-    @staticmethod
-    def getNormalizedIntensityVector(data,mzs,rtstarts,rtends,resolution,q=None):
-        """
-        Get a list of EIC vectors from a single sample
-        @param data: rawData, rawData object to extract EICs for
-        @param mzs: list, list of m/z values to get EICs for
-        @param rtstarts: list, of retention times values that are the lower bound of the EIC window
-        @param rtends: list, of retention times values that are the upper bound of the EIC window
-        @param resolution: int, number of data points to sample in the EIC window
-        @param q: Queue or None, only used for multiprocessing
-        @return: numpy array, array of EICs (one row per EIC)
-        """
-        out = np.zeros((len(mzs),resolution))
-        i=0
-        for mz,rt_start,rt_end in zip(mzs,rtstarts,rtends):
-            s = data.interpolate_data(mz,rt_start,rt_end)
-            out[i,:] = s(np.linspace(rt_start,rt_end,resolution))
-            i += 1
-        if type(q) != type(None):
-            q.put(0)
-        return out
-
-    def makeDataMatrix(self,rawdatas,mzs,rts,align=False):
-        """
-        make a matrix of EICs that is composed of every EIC for each feature in each file
-        @param rawdatas: list of rawData objects, samples to generate EICs from
-        @param mzs: list, list of m/z values to get EICs for
-        @param rts: list,  list of retention time values to get EICs for
-        @param align: bool, whether to perform retention time alignment or not (True = align, False = do not align)
-        @return: numpy matrix, matrix of EICs. The order of the matrix is first by samples then by features. For example, for an ouput matrix generated from n samples and m features, would have length n * m and the EIC for the ith feature for the jth sample would be in row: i + (j * m)
-        """
-        #gather start and end times of EIC windows
-        rtstarts = [rt - self.windowSize/2 for rt in rts]
-        rtends = [rt + self.windowSize/2 for rt in rts]
-
-        #gather arguments for function
-        args = []
-        featInds = []
-        for rawdata in rawdatas:
-            featInds += list(range(len(mzs)))
-            args.append([rawdata, mzs, rtstarts, rtends,self.resolution])
-
-        #get EICs
-        result = startConcurrentTask(PeakDetective.getNormalizedIntensityVector, args, self.numCores, "forming matrix", len(args))
-
-        #concatenate EICs
-        result = np.concatenate(result,axis=0)
-
-        #align EICs
-        if align:
-            result = alignDataMatrix(result,featInds,True,self.numCores)
-
-        return result
-
-    def trainSmoother(self,peaks,raw_datas,numPeaks,smooth_epochs,batch_size,validation_split):
-        """
-        Train smoothing autoencoder network
-        @param peaks: Pandas DataFrame, list of features detected from some peak detection software
-        @param raw_datas: list of rawData objects, samples to use for training
-        @param numPeaks: int, number of peaks to sample to train autoencoder
-        @param smooth_epochs: int, number of epochs to train for
-        @param batch_size: int, batch size for training
-        @param validation_split: float, fraction of EICs to hold out for validation, between 0-1.
-        @return: None
-        """
-        #generate data matrix
-        print("generating EICs...")
-        mzs = rd.choices(list(peaks["mz"].values),k=int(numPeaks/len(raw_datas)))
-        rts = rd.choices(list(peaks["rt"].values),k=int(numPeaks/len(raw_datas)))
-
-        X = self.makeDataMatrix(raw_datas,mzs,rts)
-
-        #normalize matrix
-        X_norm = normalizeMatrix(X)
-
-        print("done")
-
-        #fit autoencoder
-        print("fitting smoother...")
-        smoother = Smoother(self.resolution)
-        smoother.fit(X_norm, X_norm, epochs=smooth_epochs, batch_size=batch_size, validation_split=validation_split,verbose=1)
-
-        #set updated models
-        self.smoother = smoother
-        self.encoder = keras.Model(smoother.input, smoother.layers[7].output)
-        print("done")
-
-    def trainClassifier(self,X,y,X_val,y_val,min_epochs,max_epochs,batch_size,restarts):
-        """
-        Train classifer network
-        @param X: numpy matrix, input EICs to train on
-        @param y: numpy matrix, input labels to train on
-        @param X_val: numpy matrix, EICs to use a validation data
-        @param y_val: numpy matrix, input labels to use as validation
-        @param min_epochs: int, minimum number of epochs to train
-        @param max_epochs: int, maximum number of epochs to train
-        @param batch_size: int, batch size to use when training
-        @param restarts: int, number of random restarts to run
-        @return: EarlyStopping callback, training history in keras callback object
-        """
-
-        #normalize matrix
-        X_norm = normalizeMatrix(X)
-
-        #calculate peak areas
-        tics = np.log10(np.array([np.max([2, integratePeak(x)]) for x in X]))
-
-        #get latent rep. of EICs
-        X_latent = self.encoder.predict(X_norm)
-
-        #normalize validation EICs
-        X_tmp = normalizeMatrix(X_val)
-
-        #get peak areas for validation data
-        tic_val = np.log10(np.array([np.max([2, integratePeak(x)]) for x in X_val]))
-
-        #get latent rep. of validaiton EICs
-        X_val = self.encoder.predict(X_tmp)
-
-
-        #begin training
-        bestLoss = np.inf
-        bestWeights = -1
-        bestValErr = -1
-        bestBestEpoch = -1
-        trainErr = -1
-        trainLoss = -1
-
-        #iterate over random restarts
-        for x in range(restarts):
-
-            #make callback object
-            cb = keras.callbacks.EarlyStopping(
-                monitor="val_loss",
-                min_delta=0,
-                patience=3,
-                verbose=0,
-                mode="auto",
-                baseline=None,
-                restore_best_weights=True,
-            )
-
-            history = keras.callbacks.History()
-
-            # initialize classifier
-            classifer = ClassifierLatent(X_latent.shape[1])
-
-            #train to minimum epochs
-            if min_epochs > 0:
-                classifer.fit([X_latent,tics],y,epochs=int(min_epochs),batch_size=batch_size,verbose=0,
-                              validation_data=([X_val, tic_val], y_val))
-
-            #train until maximum epochs with early stopping
-            classifer.fit([X_latent, tics], y, epochs=int(max_epochs-min_epochs),
-                          batch_size=batch_size, verbose=0, callbacks=[cb, history],
-                          validation_data=([X_val, tic_val], y_val))
-
-            #get performance
-            valLoss = history.history["val_loss"][cb.best_epoch]
-            valErr = history.history["val_mean_absolute_error"][cb.best_epoch]
-            bestEpoch = cb.best_epoch
-
-            #update best performers
-            if valLoss < bestLoss:
-                bestLoss = valLoss
-                bestWeights = classifer.get_weights()
-                bestValErr = valErr
-                bestBestEpoch = bestEpoch
-                trainLoss = history.history["loss"][cb.best_epoch]
-                trainErr = history.history["mean_absolute_error"][cb.best_epoch]
-
-        #print performance
-        print("loss:",trainLoss,"mean_absolute_error:",trainErr,"val loss:", bestLoss, "val_mean_absolute_error:",bestValErr, "numEpochs:", min_epochs + bestBestEpoch)
-
-        #set best weights
-        classifer.set_weights(bestWeights)
-
-        self.classifier = classifer
-
-        return history
-
-    def trainClassifierActive(self,X,X_labeled,y_labeled,min_epochs,max_epochs,batch_size,restarts,numVal = 10,numManualPerRound=3,inJupyter=True):
-        trainingInds = []
-
-        valInds = list(range(len(X)))
-        valInds = rd.sample(valInds,numVal)
-
-        y = np.zeros((len(X)-numVal,2))
-
-        X_val = X[valInds]
-        y_val = np.zeros((numVal,2))
-
-        X = X[[x for x in range(len(X)) if x not in valInds]]
-
-        updatingInds = list(range(len(X)))
-
-        for ind in range(len(X_val)):
-            val = self.labelPeak([X_val[ind]], -1*self.windowSize/2, self.windowSize/2, inJupyter,"","relative retention time")
-            y_val[ind, 0] = 1 - val
-            y_val[ind, 1] = val
-
-
-        if len(X_labeled) > 0:
-            self.trainClassifier(X_labeled,
-                                 y_labeled,
-                                 X_val,y_val, min_epochs,max_epochs, batch_size, restarts)
-
-        y[updatingInds] = self.classifyMatrix(X[updatingInds])
-
-        doMore = True
-        i=0
-
-        def padVal(val):
-            if val < 0.5:
-                return val + 1e-8
-            else:
-                return val - 1e-8
-
-        while doMore:
-            if len(updatingInds) > 0:
-
-                entropies = [-1 * np.sum([padVal(val) * np.log(padVal(val)) for yyy in yy]) for yy in y[updatingInds]]
-
-                order = list(range(len(updatingInds)))
-                order.sort(key=lambda x: entropies[x], reverse=True)
-                order = [updatingInds[x] for x in order]
-
-                if len(order) < numManualPerRound:
-                    numManualPerRound = len(order)
-
-                inds = np.random.choice(order,numManualPerRound,replace=False,p=np.array(entropies) / np.sum(entropies))
-
-                #inds = order[:numManualPerRound]
-
-                for ind in inds:
-                    val = self.labelPeak([X[ind]], -1*self.windowSize/2, self.windowSize/2, inJupyter, y[ind][1],"relative retention time")
-                    y[ind, 0] = 1 - val
-                    y[ind, 1] = val
-                    trainingInds.append(ind)
-                    updatingInds.remove(ind)
-
-                if len(X_labeled) > 0:
-                    X_train = np.concatenate((X[trainingInds],X_labeled),axis=0)
-                    y_train = np.concatenate((y[trainingInds],y_labeled),axis=0)
-                else:
-                    X_train = X[trainingInds]
-                    y_train = y[trainingInds]
-
-                if len(X_train) > 0:
-                    self.trainClassifier(X_train,y_train,X_val,y_val,min_epochs,max_epochs,batch_size,restarts)
-
-                y[updatingInds] = self.classifyMatrix(X[updatingInds])
-
-                plt.figure()
-                plt.hist(y[:, 1], bins=20)
-                plt.title("round" + str(i + 1))
-                plt.xlabel("PeakDetective Score")
-                plt.ylabel("Number of features")
-                plt.show()
-
-                print(str(len(updatingInds)) + " unclassified features remaining")
-                print("Continue with another iteration? (1=Yes, 0=No): ")
-                tmp = float(input())
-                while not validateInput(tmp):
-                    print("invalid classification: ")
-                    tmp = float(input())
-                doMore = bool(tmp)
-
-            else:
-                doMore = False
-            i += 1
-
-        plotScoringStatistics(self.classifyMatrix(X_val)[:,1],y_val[:,1])
-
-
-    def classifyMatrix(self,X):
-        # normalize matrix
-        X_norm = normalizeMatrix(X)
-        peak_areas = np.log10(np.array([np.max([2, integratePeak(x)]) for x in X]))
-
-        X_latent = self.encoder.predict(X_norm)
-        y = self.classifier.predict([X_latent, peak_areas])
-        return y
-
-    def curatePeaks(self,raw_datas,peaks,threshold=0.5,align=False):
-        print("generating EICs...")
-        mzs = peaks["mz"].values
-        rts =  peaks["rt"].values
-
-        X = self.makeDataMatrix(raw_datas,mzs,rts,align=align)
-
-        y = self.classifyMatrix(X)
-
-        peak_curated = deepcopy(peaks)
-        peak_scores = deepcopy(peaks)
-        peak_intensities = deepcopy(peaks)
-
-        keys = []
-        for raw in raw_datas:
-            peak_scores[raw.filename] = np.zeros(len(peak_scores.index.values))
-            peak_intensities[raw.filename] = np.zeros(len(peak_scores.index.values))
-            for index in peaks.index.values:
-                keys.append([raw.filename, index])
-
-        for [file, index], score in zip(keys, y[:, 1]):
-            peak_scores.at[index, file] = score
-            val = 0
-            if score > threshold:
-                val = 1
-            peak_curated.at[index, file] = val
-
-        peak_intensities = self.performIntegration(X, [raw.filename for raw in raw_datas], peak_scores, threshold)
-
-        return peak_curated,peak_scores,peak_intensities
-
-    def detectPeaks(self, rawDatas, cutoff=0.5, intensityCutoff = 100,numDataPoints=3,window=0.05,align=True,detectFrac=0.0):
-        rois = self.roiDetection(rawDatas, intensityCutoff=intensityCutoff, numDataPoints=numDataPoints)
-
-        print("generating all EICs from ROIs...")
-        dt = self.windowSize / self.resolution
-        tmpRes = int(math.ceil((rawDatas[0].rts[-1] - rawDatas[0].rts[0] + self.windowSize) / dt))
-        oldRes = int(self.resolution)
-        oldwindow = float(self.windowSize)
-        self.resolution = tmpRes
-        self.windowSize = rawDatas[0].rts[-1] + self.windowSize/2 - rawDatas[0].rts[0] + self.windowSize/2
-        rts = [(rawDatas[0].rts[-1] + rawDatas[0].rts[0])/2 for _ in rois]
-        X_tot = self.makeDataMatrix(rawDatas, rois, rts,align)
-        self.resolution = oldRes
-        self.windowSize = oldwindow
-
-
-        numPoints = 0
-        rt = rawDatas[0].rts[0]
-        while(rt <= rawDatas[0].rts[-1]):
-            numPoints += 1
-            rt += window
-
-        X = np.zeros((int(numPoints * len(rois) * len(rawDatas)), self.resolution))
-
-
-        mzs = []
-        rts = []
-        files = []
-        featInds = []
-
-
-        counter = 0
-        rowCounter = 0
-        trueDt = tmpRes / (rawDatas[0].rts[-1] + self.windowSize/2 - rawDatas[0].rts[0] + self.windowSize/2)
-        stride = int(np.floor(window * trueDt))
-
-        for rawData in rawDatas:
-            i = 0
-            for row in range(len(rois)):
-                rt = float(rawDatas[0].rts[0])
-                start = 0
-                end = start + self.resolution
-                for _ in range(numPoints):
-                    if end >= X_tot.shape[1]:
-                        n = X_tot.shape[1] - start
-                        print(start,end,n,X.shape,X_tot.shape,numPoints)
-                        X[counter,:n]  = X_tot[rowCounter,start:]
-                    else:
-                        X[counter, :] = X_tot[rowCounter, start:end]
-                    counter += 1
-                    start += stride
-                    end += stride
-                    mzs.append(rois[row])
-                    rts.append(rt)
-                    rt += window
-                    files.append(rawData.filename)
-                    featInds.append(i)
-                    i += 1
-                rowCounter += 1
-
-        X = X[:counter]
-
-        print(len(X),"EICs constructed for evaluation")
-
-        peak_areas = [integratePeak(x) for x in X]
-        toClassify = [x for x in range(len(peak_areas)) if peak_areas[x] > intensityCutoff]
-
-        peak_scores = pd.DataFrame(index=range(len(set(featInds))))
-
-        orderedMzs = []
-        orderedRts = []
-
-        for row in range(len(rois)):
-            rt = float(rawDatas[0].rts[0])
-            for _ in range(numPoints):
-                orderedMzs.append(rois[row])
-                orderedRts.append(rt)
-                rt += window
-
-        peak_scores["mz"] = orderedMzs
-        peak_scores["rt"] = orderedRts
-
-        for rawData in rawDatas:
-            peak_scores[rawData.filename] = 0.0
-
-        y = np.zeros(len(X))
-        y[toClassify] = self.classifyMatrix(X[toClassify])[:, 1]
-        print("done")
-
-        goodInds = []
-        for id,filename, score in zip(featInds,files, y):
-            if score > cutoff:
-                goodInds.append(id)
-            peak_scores.at[id,filename] = score
-
-        detectNum = int(np.ceil(len(rawDatas) * detectFrac))
-        counts = {x:0 for x in list(set(goodInds))}
-        for x in goodInds:
-            counts[x] += 1
-        goodInds = [x for x in counts if counts[x] >= detectNum]
-        goodInds.sort()
-
-
-        toKeep = []
-        for x in range(len(rawDatas)):
-            for g in goodInds:
-                toKeep.append(x*len(peak_scores) + g)
-
-        X = X[toKeep]
-
-        peak_scores = peak_scores.loc[goodInds,:]
-
-        peak_scores = peak_scores.reset_index()
-
-        apex_rts = self.updateRT(peak_scores,[raw.filename for raw in rawDatas],X,cutoff)
-
-        peak_scores["rt"] = np.round(apex_rts,2)
-
-        apex_mzs = self.updateMz(peak_scores,rawDatas,cutoff)
-
-        peak_scores["mz"] = np.round(apex_mzs,7)
-
-        peak_intensities = self.performIntegration(X, [raw.filename for raw in rawDatas], peak_scores, cutoff)
-
-        peak_intensities = peak_intensities.drop_duplicates(["mz","rt"],keep="first")
-        peak_scores = peak_scores.drop_duplicates(["mz","rt"],keep="first")
-
-        print(len(peak_scores), " peaks found")
-
-        return peak_scores, peak_intensities, rois
-
-    def updateRT(self,peakScores,samples,X,cutoff,smooth=False):
-        i = 0
-        rts = []
-        dt = self.windowSize / self.resolution
-        for index, row in peakScores.iterrows():
-            inds = []
-            allInds = []
-            for n,samp in enumerate(samples):
-                ind = i + n * len(peakScores)
-                if row[samp] > cutoff:
-                    inds.append(ind)
-                allInds.append(ind)
-            if len(inds) > 0:
-                tmp = X[inds].sum(axis=0)
-                if smooth: tmp = self.smoother.predict(normalizeMatrix(np.array([tmp])), verbose=0)[0]
-                lb, rb, apex = findPeakBoundaries(tmp)
-
-            else:
-                apex = (self.resolution-1)/2
-
-            rt = (apex - (self.resolution-1)/2) * dt + row["rt"]
-            rts.append(rt)
-            i += 1
-            printProgressBar(i, len(peakScores), "refining retention times", printEnd="")
-
-        return rts
-
-    def updateMz(self,peak_scores,raw_data,cutoff):
-        mzs = []
-        i = 0
-        for index,row in peak_scores.iterrows():
-            tmp = []
-            for data in raw_data:
-                if row[data.filename] > cutoff:
-                    tmp.append(data.getApexMz(row["mz"],row["rt"]))
-            tmp = np.array(tmp)
-            mzs.append(np.average(tmp[:,0],weights=tmp[:,1]))
-            i += 1
-            printProgressBar(i, len(peak_scores), "refining mzs", printEnd="")
-        return mzs
-
-    def label_peaks(self,raw_data,peaks,inJupyter = True):
-        rt_starts = [row["rt"] - self.windowSize/2 for _,row in peaks.iterrows()]
-        rt_ends = [row["rt"] + self.windowSize/2 for _,row in peaks.iterrows()]
-        y = []
-        mat = self.makeDataMatrix([raw_data],peaks["mz"].values,peaks['rt'])
-        count = 1
-        for vec,rt_start,rt_end in zip(mat,rt_starts,rt_ends):
-            y.append(self.labelPeak([vec],rt_start,rt_end,inJupyter,str(count) + "/" + str(len(mat)),"retention time"))
-            count += 1
-        peaks["classification"] = y
-        return peaks
-
-    def labelPeak(self,vecs,rt_start,rt_end,inJupyter,title="",xlabel="retention time"):
-        plt.figure()
-        plt.ion()
-        xs = np.linspace(rt_start, rt_end, len(vecs[0]))
-        [plt.plot(xs, vec) for vec in vecs]
-        plt.xlabel(xlabel)
-        plt.ylabel("intensity")
-        plt.title(title)
-        plt.show(block=False)
-        plt.pause(0.001)
-        print("Enter classification (1=True Peak, 0=Artifact): ")
-        val = input()
-
-        while not validateInput(val):
-            print("invalid classification: ")
-            val = input()
-        val = float(val)
-        plt.close()
-        if inJupyter:
-            IPython.display.clear_output(wait=True)
-
-        return val
-
-    def roiDetection(self,rawdatas,intensityCutoff=100,numDataPoints = 3):
-        rtss = [rawdata.rts for rawdata in rawdatas]
-        rois = []
-
-        counter = 0
-        totalNum = np.sum([len(rts) for rts in rtss])
-        for rts,rawdata in zip(rtss,rawdatas):
-            ppm = rawdata.ppm
-            for rt in rts:
-                printProgressBar(counter, totalNum,prefix = "Detecting ROIs",suffix=str(len(rois)) + " ROIs found",printEnd="")
-                counter += 1
-                for mz, i in rawdata.data[rt]:
-                    if i > intensityCutoff:
-                        update,pos = binarySearchROI(rois,mz,ppm)
-                        if update:
-                            rois[pos]["mzs"].append(mz)
-                            rois[pos]["mz_mean"] = np.mean(rois[pos]["mzs"])
-                            rois[pos]["extended"] = True
-                            rois[pos]["count"] += 1
-                        else:
-                            if pos != len(rois):
-                                rois.insert(pos,{"mz_mean":mz,"mzs":[mz],"extended":True,"count":1})
-                            else:
-                                rois.append({"mz_mean":mz,"mzs":[mz],"extended":True,"count":1})
-
-            toKeep = []
-            for x in range(len(rois)):
-                if rois[x]["extended"] == True or rois[x]["count"] >= numDataPoints:
-                    toKeep.append(x)
-
-            rois = [rois[x] for x in toKeep]
-
-            for x in range(len(rois)):
-                rois[x]["extended"] = False
-
-
-        rois = [x["mz_mean"] for x in rois]
-        print()
-        print(len(rois)," ROIs found")
-
-        return rois
-
-    def filterPeakListByScores(self,peakScores,samples,cutoff,frac):
-        goodInds = [index for index,row in peakScores.iterrows() if float(len([x for x in samples if row[x] > cutoff])) / len(samples) > frac]
-        return peakScores.loc[goodInds,:]
-
-    def performIntegration(self, X, samples, peakScores, cutoff, defaultWidth=0.5,smooth=False):
-        i = 0
-        peak_areas = pd.DataFrame(index=peakScores.index.values,columns=["mz","rt"])
-        peak_areas["mz"] = peakScores["mz"].values
-        peak_areas["rt"] = peakScores["rt"].values
-        peak_areas[samples] = np.zeros(peakScores[samples].values.shape)
-        print("integrating peaks...")
-        for index,row in peakScores.iterrows():
-            inds = []
-            allInds = []
-            for n,samp in enumerate(samples):
-                ind = i + n * len(peakScores)
-                if row[samp] > cutoff:
-                    inds.append(ind)
-                allInds.append(ind)
-            if len(inds) > 0:
-                tmp = X[inds].sum(axis=0)
-                if smooth: tmp = self.smoother.predict(normalizeMatrix(np.array([tmp])),verbose=0)[0]
-                lb,rb,apex = findPeakBoundaries(tmp)
-            else:
-                lb = int(np.round(self.resolution / 2 - defaultWidth * self.resolution / 2))
-                rb = int(np.round(self.resolution/2 + defaultWidth * self.resolution/2))
-            for ind,sample in zip(allInds,samples):
-                peak_areas.at[index,sample] = integratePeak(X[ind],[lb,rb])
-            i += 1
-            printProgressBar(i, len(peakScores), "integrating peaks", printEnd="")
-
-        return peak_areas
-
-
-class rawData():
-    def __init__(self,data={},filename="",ppm=0,timestamp=None):
-        self.data = data
-        self.filename = filename
-        self.rts = list(self.data.keys())
-        self.rts.sort()
-        self.ppm = ppm
-        self.timestamp = None
-
-    def readRawDataFile(self,filename,ppm,intensityThresh = 0):
-        """
-         Read MS datafile
-
-        :param filename: str, path to MS datafile
-        """
-        try:
-            try:
-                with mzml.MzML(filename.replace('"', "")) as f:
-                    self.timestamp = datetime.datetime.fromisoformat(next(f.iterfind('run', recursive=False))['startTimeStamp'][:-1]).astimezone(datetime.timezone.utc)
-            except:
-                print("Warning: file timestamp could not be read")
-                self.timestamp = None
-            reader = mzml.read(filename.replace('"', ""))
-            ms1Scans = {}
-            for temp in reader:
-                if temp['ms level'] == 1:
-                    spectrum = [[mz,i] for mz, i in zip(temp["m/z array"],temp["intensity array"]) if i > intensityThresh]
-                    spectrum.sort(key=lambda x:x[0])
-                    ms1Scans[temp["scanList"]["scan"][0]["scan start time"]] = spectrum
-            reader.close()
-            self.rts = list(ms1Scans.keys())
-            self.rts.sort()
-            self.data = ms1Scans
-            self.filename = filename
-            self.ppm = ppm
-
-        except:
-            print(sys.exc_info())
-            print(filename + " does not exist or is ill-formatted")
-
-
-    def extractEIC(self,mz,rt_start,rt_end):
-        width = self.ppm * mz / 1e6
-        mz_start = mz - width
-        mz_end = mz + width
-        rts = [x for x in self.rts if x > rt_start and x < rt_end]
-        intensity = []
-        for rt in rts:
-            Origind = getIndexOfClosestValue([x[0] for x in self.data[rt]],mz)
-            ind = int(Origind)
-            tmp = 0
-            while  ind < len(self.data[rt]) and self.data[rt][ind][0] > mz_start and self.data[rt][ind][0] < mz_end:
-                tmp += self.data[rt][ind][1]
-                ind += 1
-            ind = Origind - 1
-            while ind > -1 and self.data[rt][ind][0] > mz_start and self.data[rt][ind][0] < mz_end :
-                tmp += self.data[rt][ind][1]
-                ind -= 1
-            intensity.append(tmp)
-        return rts,intensity
-
-    def getApexMz(self,mz,rt):
-        width = self.ppm * mz / 1e6
-        mz_start = mz - width
-        mz_end = mz + width
-        rt = self.rts[getIndexOfClosestValue(self.rts,rt)]
-        highestMz = mz
-        highestIntensity = 1
-        Origind = getIndexOfClosestValue([x[0] for x in self.data[rt]], mz)
-        ind = int(Origind)
-        while ind < len(self.data[rt]) and self.data[rt][ind][0] > mz_start and self.data[rt][ind][0] < mz_end:
-            if self.data[rt][ind][1] > highestIntensity:
-                highestIntensity = self.data[rt][ind][1]
-                highestMz = self.data[rt][ind][0]
-            ind += 1
-        ind = Origind - 1
-        while ind > -1 and self.data[rt][ind][0] > mz_start and self.data[rt][ind][0] < mz_end:
-            if self.data[rt][ind][1] > highestIntensity:
-                highestIntensity = self.data[rt][ind][1]
-                highestMz = self.data[rt][ind][0]
-            ind -= 1
-        return highestMz,highestIntensity
-
-    def interpolate_data(self,mz,rt_start,rt_end):
-        rts,intensity = self.extractEIC(mz,rt_start,rt_end)
-        if len(rts) > 3:
-            #smoothing = smoothing * len(rts) * np.max(intensity)
-            #s = UnivariateSpline(rts,intensity,ext=1,s=smoothing)
-            s = interp1d(rts,intensity,kind="linear",fill_value=0,bounds_error=False)
-        else:
-            #s = UnivariateSpline([0,5,10,15],[0,0,0,0],ext=1,s=smoothing)
-            s = interp1d([0,5,10,15],[0,0,0,0],kind="linear",fill_value=0,bounds_error=False)
-
-        return s
-
-    def getMergedSpectrum(self,rtRange=None,intensityThresh=0,ppm=1):
-        if rtRange is None:
-            rtRange = [self.rts[0],self.rts[-1]]
-        spectra = [[[mz,i] for mz,i in self.data[rt] if i > intensityThresh] for rt in self.rts if rt > rtRange[0] and rt < rtRange[1]]
-        return mergeSpectra(spectra,ppm)
-
-
-def Smoother(resolution):
-    # build autoencoder
-    autoencoderInput = keras.Input(shape=(resolution,))
-    x = layers.Reshape((resolution, 1))(autoencoderInput)
-
-    kernelsize = 3
-    stride = 1
-    max_norm_value = 2.0
-
-    x = layers.Conv1D(32, kernelsize, strides=stride, activation='relu', kernel_constraint=max_norm(max_norm_value),
-                     kernel_initializer='he_uniform')(x)
-
-    #x = layers.BatchNormalization()(x)
-
-    x = layers.Conv1D(16, kernelsize, strides=stride, activation='relu', kernel_constraint=max_norm(max_norm_value),
-                     kernel_initializer='he_uniform')(x)
-
-    #x = layers.BatchNormalization()(x)
-
-    x = layers.Conv1D(8, kernelsize, strides=stride, activation='relu', kernel_constraint=max_norm(max_norm_value),
-                      kernel_initializer='he_uniform')(x)
-
-    #x = layers.BatchNormalization()(x)
-
-    x = layers.Conv1D(4, kernelsize, strides=stride, activation='relu', kernel_constraint=max_norm(max_norm_value),
-                      kernel_initializer='he_uniform')(x)
-
-    #x = layers.BatchNormalization()(x)
-
-    x = layers.Flatten()(x)
-
-    x = layers.Dense(5, activation="relu")(x)
-
-    x = layers.Dense(int((resolution-8) * 4), activation="relu")(x)
-
-    x = layers.Reshape((resolution-8, 4))(x)
-
-    x = layers.Conv1DTranspose(8, kernelsize, strides=stride, activation='relu',
-                               kernel_constraint=max_norm(max_norm_value), kernel_initializer='he_uniform')(x)
-
-    #x = layers.BatchNormalization()(x)
-
-    x = layers.Conv1DTranspose(16, kernelsize, strides=stride, activation='relu',
-                              kernel_constraint=max_norm(max_norm_value), kernel_initializer='he_uniform')(x)
-
-    #x = layers.BatchNormalization()(x)
-
-    x = layers.Conv1DTranspose(32, kernelsize, strides=stride, activation='relu',
-                              kernel_constraint=max_norm(max_norm_value), kernel_initializer='he_uniform')(x)
-
-    #x = layers.BatchNormalization()(x)
-
-    x = layers.Conv1DTranspose(1, kernelsize, strides=stride, activation='sigmoid',
-                               kernel_constraint=max_norm(max_norm_value), kernel_initializer='he_uniform')(x)
-
-    x = layers.Flatten()(x)
-
-    autoencoder = keras.Model(autoencoderInput, x)
-
-    autoencoder.compile(loss='binary_crossentropy', optimizer=keras.optimizers.Adam(1e-4),
-                        metrics=['mean_absolute_error'],weighted_metrics=[])
-
-
-    return autoencoder
-
-def ClassifierLatent(resolution):
-    descriminatorInput = keras.Input(shape=(resolution,))
-    ticInput = keras.Input(shape=(1,))
-
-    #x = layers.Dense(resolution, activation="relu")(descriminatorInput)
-
-    x = layers.Layer()(descriminatorInput)
-
-    x = keras.Model(descriminatorInput, x)
-
-    tic = keras.Model(ticInput, layers.Layer()(ticInput))
-
-    x = layers.concatenate([x.output, tic.output], axis=1)
-
-    x = layers.Dense(int(resolution), activation="relu")(x)
-
-    x = layers.Dense(int(resolution), activation="relu")(x)
-
-    x = layers.Dense(int(resolution), activation="relu")(x)
-
-    x = layers.Dense(int(resolution), activation="relu")(x)
-
-    x = layers.Dense(int(resolution), activation="relu")(x)
-
-    output = layers.Dense(2, activation="softmax")(x)
-
-    classifier = keras.Model([descriminatorInput, ticInput], output, name="discriminator")
-
-    classifier.compile(loss='binary_crossentropy', optimizer=keras.optimizers.Adam(1e-4),
-                          metrics=['mean_absolute_error'])
-
-    return classifier
-
-
-def makePRCPlot(pred,true,noSkill=True):
-
-    prec, recall, threshs = met.precision_recall_curve(true, pred)
-
-    auc = np.round(met.auc(recall, prec), 4)
-
-    plt.plot(recall, prec, label="prAUC=" + str(auc))
-    plt.xlabel("Recall")
-    plt.ylabel("Precision")
-    if noSkill:
-        numPositive = len([x for x in true if x > 0.5])
-        numNegative = len(true) - numPositive
-        plt.plot([0, 1.0],
-                 [numPositive / float(numPositive + numNegative), numPositive / float(numPositive + numNegative)],
-                 label="NSL prAUC=" + str(
-                     np.round(numPositive / float(numPositive + numNegative), 4)))
-    plt.legend()
-    return auc
-
-
-def findPeakBoundaries(peak):
-    apex = int(len(peak)/2)
-    #find left bound
-
-    foundNewApex = True
-
-    while(foundNewApex):
-        foundNewApex = False
-
-        x = apex
-        while peak[x] > peak[apex] / 2 and x > 0:
-            if peak[x] > peak[apex]:
-                apex = x
-            x -= 1
-        lb = x
-
-        x = apex
-        while peak[x] > peak[apex] / 2 and x < len(peak) - 1:
-            if peak[x] > peak[apex]:
-                apex = x
-                foundNewApex = True
-            x += 1
-        rb = x
-
-    return lb,rb,apex
-
-def integratePeak(peak,bounds=None):
-    if bounds is None:
-        lb,rb,apex = findPeakBoundaries(peak)
-    else:
-        lb = bounds[0]
-        rb = bounds[1]
-    if lb != rb:
-        try:
-            area = np.trapz(peak[lb:rb],np.linspace(lb,rb,rb-lb))
-        except:
-            print(lb,rb)
-            area = 0
-    else:
-        area = 0
-    return area
-
-
-def alignPeaks(peaks,normalize=True,reference=0,q=None):
-    if normalize:
-        peaks_norm = [safeNormalize(x) for x in peaks]
-    else:
-        peaks_norm = deepcopy(peaks)
-
-    reference_peak = peaks_norm[reference]
-    ref = list(range(len(reference_peak)))
-
-    for x,peak in enumerate(peaks_norm):
-        if x > 0:
-            distance, path = fastdtw(np.array(reference_peak).flatten(), np.array(peak).flatten(), dist=2)
-            xs = []
-            ys = []
-
-            prev = path[0][0]
-            tmp = [peaks[x][path[0][1]]]
-            for p1,p2 in path[1:]:
-                if p1 != prev:
-                    xs.append(prev)
-                    ys.append(np.mean(tmp))
-                    tmp = []
-                tmp.append(peaks[x][p2])
-                prev = p1
-            xs.append(prev)
-            ys.append(np.mean(tmp))
-
-
-            f = interp1d(xs,ys,fill_value=0.0,bounds_error=False)
-            peaks[x] = [f(i) for i in ref]
-
-
-    if type(q) != type(None):
-        q.put(0)
-
-    return peaks
-
-def alignDataMatrix(matrix,peakInds,normalize=True,numCores=1):
-    uniquePeaks = list(set(peakInds))
-    order = [[] for _ in uniquePeaks]
-    args = [[[],normalize,0] for _ in uniquePeaks]
-    for i,peak,ind in zip(range(len(matrix)),matrix,peakInds):
-        args[ind][0].append(peak)
-        order[ind].append(i)
-    result = startConcurrentTask(alignPeaks,args,numCores,"aligning EICs",len(uniquePeaks))
-    for peaks,inds in zip(result,order):
-        for peak,ind in zip(peaks,inds):
-            matrix[ind] = peak
-    return matrix
-
-
-def takeClosestInd(myList, myNumber):
-    """
-    Assumes myList is sorted. Returns closest value to myNumber.
-
-    If two numbers are equally close, return the smallest number.
-    """
-
-    pos = bisect_left(myList, myNumber)
-    if pos == 0:
-        return pos
-    if pos == len(myList):
-        return len(myList) - 1
-    before = myList[pos - 1]
-    after = myList[pos]
-    if after - myNumber < myNumber - before:
-        return pos
-    else:
-        return pos-1
-
-def mergeSpectra(spectra,ppm):
-    if len(spectra) > 0:
-        mergedSpectrumMzs = [x[0] for x in spectra[0]]
-        mergedSpectrumInts = [x[1] for x in spectra[0]]
-
-        if len(spectra) > 1:
-            fact = ppm / 1e6
-            for spectrum in spectra[1:]:
-                for mz,i in spectrum:
-                    if len(mergedSpectrumMzs) > 0:
-
-                        x = takeClosestInd(mergedSpectrumMzs,mz)
-                        delta = mz * fact
-
-                        if mergedSpectrumMzs[x] > mz - delta and mergedSpectrumMzs[x] < mz + delta:
-                            mergedSpectrumInts[x] += i
-                        else:
-                            if mz < mergedSpectrumMzs[x]:
-                                mergedSpectrumMzs.insert(x,mz)
-                                mergedSpectrumInts.insert(x,i)
-                            else:
-                                mergedSpectrumMzs.insert(x+1,mz)
-                                mergedSpectrumInts.insert(x+1,i)
-
-                    else:
-                        mergedSpectrumMzs.append(mz)
-                        mergedSpectrumInts.append(i)
-    else:
-        mergedSpectrumMzs = []
-        mergedSpectrumInts = []
-
-
-    return [[mz,i] for mz,i in zip(mergedSpectrumMzs,mergedSpectrumInts)]
-
-#Utility functions:
-
-#runs a function concurently.
-def startConcurrentTask(task,args,numCores,message,total,chunksize="none",verbose=True):
-
-    if verbose:
-        m = Manager()
-        q = m.Queue()
-        args = [a + [q] for a in args]
-        t = Thread(target=updateProgress, args=(q, total, message))
-        t.start()
-    if numCores > 1:
-        p = Pool(numCores)
-        if chunksize == "none":
-            res = p.starmap(task, args)
-        else:
-            res = p.starmap(task, args, chunksize=chunksize)
-        p.close()
-        p.join()
-    else:
-        res = [task(*a) for a in args]
-    if verbose: t.join()
-    return res
-
-
-def safeNormalize(x):
-    """
-    Safely normalize a vector, x, to sum to 1.0. If x is the zero vector return the normalized unity vector
-    """
-    if np.sum(x) < 1e-6:
-        tmp = np.ones(x.shape)
-        return tmp / np.sum(tmp)
-    else:
-        return x/np.sum(x)
-
-def normalizeMatrix(X):
-    """
-    Normalize a matrix so that the rows of X sum to one
-    """
-    return np.array([safeNormalize(x) for x in X])
-
-def classify(preds):
-    """
-    Classify predictions, preds, by returning the index of the highest scoring class
-    """
-    classes = np.zeros(preds.shape)
-    for x in range(len(preds)):
-        classes[x,list(preds[x]).index(np.max(list(preds[x])))] = 1
-    return classes
-
-
-def take_closest(myList, myNumber):
-    """
-    Assumes myList is sorted. Returns closest value to myNumber.
-
-    If two numbers are equally close, return the smallest number.
-    """
-    pos = bisect_left(myList, myNumber)
-    if pos == 0:
-        return myList[0]
-    if pos == len(myList):
-        return myList[-1]
-    before = myList[pos - 1]
-    after = myList[pos]
-    if after - myNumber < myNumber - before:
-        return after
-    else:
-        return before
-
-
-
-def printProgressBar(iteration, total, prefix='', suffix='', decimals=1, length=50, fill='█', printEnd="\r"):
-    """
-    Call in a loop to create terminal progress bar
-    @params:
-        iteration   - Required  : current iteration (Int)
-        total       - Required  : total iterations (Int)
-        prefix      - Optional  : prefix string (Str)
-        suffix      - Optional  : suffix string (Str)
-        decimals    - Optional  : positive number of decimals in percent complete (Int)
-        length      - Optional  : character length of bar (Int)
-        fill        - Optional  : bar fill character (Str)
-        printEnd    - Optional  : end character (e.g. "\r", "\r\n") (Str)
-    """
-    percent = ("{0:." + str(decimals) + "f}").format(100 * (iteration / float(total)))
-    filledLength = int(length * iteration // total)
-    bar = fill * filledLength + '-' * (length - filledLength)
-    print(f'\r{prefix} |{bar}| {percent}% {suffix}', end=printEnd)
-    # Print New Line on Complete
-    if iteration == total:
-        print()
-
-def updateProgress(q, total,message = ""):
-    """
-    update progress bar
-    """
-    counter = 0
-    while counter != total:
-        if not q.empty():
-            q.get()
-            counter += 1
-            #if counter % 20 == 0:
-            printProgressBar(counter, total,prefix = message, printEnd="")
-
-
-def getIndexOfClosestValue(l,v):
-    """
-    get index of list with closest value to v, assumes l is sorted
-    """
-    pos = bisect_left(l, v)
-    if pos == 0:
-        return 0
-    if pos == len(l):
-        return pos - 1
-    before = l[pos - 1]
-    after = l[pos]
-    if after - v < v - before:
-        return pos
-    else:
-        return pos - 1
-
-def plotScoringStatistics(scores, labels):
-    tpr = []
-    fdr = []
-    cutoffs = np.linspace(0, 1.0, 100)
-    for cutoff in cutoffs:
-        fdr.append(1 - met.precision_score(labels, scores > cutoff, zero_division=0))
-        tpr.append(met.recall_score(labels, scores > cutoff, zero_division=0))
-    plt.scatter(cutoffs, tpr, c="black", label="TPR")
-    plt.plot(cutoffs, tpr, c="black")
-
-    plt.scatter(cutoffs, fdr, c="red", label="FDR")
-    plt.plot(cutoffs, fdr, c="red")
-    plt.legend()
-    plt.xlabel("cutoff")
-    plt.ylabel("performance")
-
-def validateInput(input):
-    """
-    Validate input, used for the labelPeaks() function
-    @param input: str, user input
-    @return: Bool, True = user input was a 0 or 1, False otherwise
-    """
-    try:
-        input = float(input)
-        if input not in [0, 1]:
-            return False
-        return True
-    except:
-        return False
-
-def binarySearchROI(poss, query, ppm):
-    """
-    Search function used in ROI calculations
-    """
-    if len(poss) == 0:
-        return False, 0
-
-    pos = bisect_left([x["mz_mean"] for x in poss], query)
-
-    if pos == len(poss):
-        if 1e6 * np.abs(query - poss[-1]["mz_mean"]) / query < ppm:
-            return True, pos - 1
-        else:
-            return False, pos
-    elif pos == 0:
-        if 1e6 * np.abs(query - poss[0]["mz_mean"]) / query < ppm:
-            return True, 0
-        else:
-            return False, pos
-    else:
-        ldiff = 1e6 * np.abs(query - poss[pos - 1]["mz_mean"]) / query
-        rdiff = 1e6 * np.abs(query - poss[pos]["mz_mean"]) / query
-
-        if ldiff < rdiff:
-            if ldiff < ppm:
-                return True, pos - 1
-            else:
-                return False, pos
-        else:
-            if rdiff < ppm:
-                return True, pos
-            else:
+from pyteomics import mzml
+import sys
+import numpy as np
+import matplotlib.pyplot as plt
+from multiprocessing import Manager,Pool
+from threading import Thread
+from tensorflow import keras
+from keras.constraints import max_norm
+import keras.layers as layers
+import scipy.stats as stats
+from bisect import bisect_left
+import math
+import random as rd
+import IPython.display
+from copy import deepcopy
+import pandas as pd
+from scipy.spatial.distance import euclidean
+from fastdtw import fastdtw
+from scipy.interpolate import interp1d
+import pickle as pkl
+import os
+import sklearn.metrics as met
+import datetime
+
+
+class PeakDetective():
+    """
+    Class for curation/detection of LC/MS peaks in untargeted metabolomics data
+    """
+    def __init__(self,resolution=60,numCores=1,windowSize = 1.0):
+        """
+        Constructor for PeakDetective object
+        @param resolution: int, number of datapoints to sample in the EIC window
+        @param numCores: int, number of processor cores to use for concurrent computations
+        @param windowSize: float, size of EIC window to extract (in minutes)
+        """
+        self.resolution = resolution
+        self.numCores = numCores
+        self.windowSize = windowSize
+        self.smoother = Smoother(resolution)
+        self.classifier = ClassifierLatent(5)
+        self.encoder = keras.Model(self.smoother.input, self.smoother.layers[7].output)
+
+    def save(self,path):
+        """
+        Save model weights to given path
+        @param path: str, path where weights should be saved
+        @return: None
+        """
+        if not os.path.exists(path): os.mkdir(path)
+        pkl.dump([self.resolution,self.windowSize],open(path+"parameters.pd","wb"))
+        self.smoother.save(path + "smoother.h5")
+        self.classifier.save(path+"classifier.h5")
+        self.encoder.save(path+"encoder.h5")
+
+
+    def load(self,path):
+        """
+        Load model weights
+        @param path: str, path to folder where model weights were saved
+        @return: None
+        """
+        try:
+            [self.resouton,self.windowSize] = pkl.load(open(path + "parameters.pd","rb"))
+            self.smoother = keras.models.load_model(path+"smoother.h5")
+            self.classifier = keras.models.load_model(path+"classifier.h5")
+            self.encoder = keras.models.load_model(path+"encoder.h5")
+
+        except:
+            print("Error: pd and h5 files were not found, check path")
+
+    def plot_overlayedEIC(self,rawdatas,mz,rt_start,rt_end,alpha=0.3):
+        """
+        Plot an overlayed EIC for specified samples and mz and retention time range
+        @param rawdatas: list of rawData objects, samples to plot EIC for
+        @param mz: float, m/z value to extract EIC
+        @param rt_start: float, retention time value that is the starting value to plot
+        @param rt_end: float, retention time value that is the ending value to plot
+        @param alpha: float, transparency factor (0-1)
+        @return: None
+        """
+        ts = np.linspace(rt_start,rt_end,self.resolution)
+        for data in rawdatas:
+            s = data.interpolate_data(mz,rt_start,rt_end)
+            ints  = [np.max([x,0]) for x in s(ts)]
+            plt.plot(ts,ints,alpha=alpha)
+
+
+    @staticmethod
+    def getNormalizedIntensityVector(data,mzs,rtstarts,rtends,resolution,q=None):
+        """
+        Get a list of EIC vectors from a single sample
+        @param data: rawData, rawData object to extract EICs for
+        @param mzs: list, list of m/z values to get EICs for
+        @param rtstarts: list, of retention times values that are the lower bound of the EIC window
+        @param rtends: list, of retention times values that are the upper bound of the EIC window
+        @param resolution: int, number of data points to sample in the EIC window
+        @param q: Queue or None, only used for multiprocessing
+        @return: numpy array, array of EICs (one row per EIC)
+        """
+        out = np.zeros((len(mzs),resolution))
+        i=0
+        for mz,rt_start,rt_end in zip(mzs,rtstarts,rtends):
+            s = data.interpolate_data(mz,rt_start,rt_end)
+            out[i,:] = s(np.linspace(rt_start,rt_end,resolution))
+            i += 1
+        if type(q) != type(None):
+            q.put(0)
+        return out
+
+    def makeDataMatrix(self,rawdatas,mzs,rts,align=False):
+        """
+        make a matrix of EICs that is composed of every EIC for each feature in each file
+        @param rawdatas: list of rawData objects, samples to generate EICs from
+        @param mzs: list, list of m/z values to get EICs for
+        @param rts: list,  list of retention time values to get EICs for
+        @param align: bool, whether to perform retention time alignment or not (True = align, False = do not align)
+        @return: numpy matrix, matrix of EICs. The order of the matrix is first by samples then by features. For example, for an ouput matrix generated from n samples and m features, would have length n * m and the EIC for the ith feature for the jth sample would be in row: i + (j * m)
+        """
+        #gather start and end times of EIC windows
+        rtstarts = [rt - self.windowSize/2 for rt in rts]
+        rtends = [rt + self.windowSize/2 for rt in rts]
+
+        #gather arguments for function
+        args = []
+        featInds = []
+        for rawdata in rawdatas:
+            featInds += list(range(len(mzs)))
+            args.append([rawdata, mzs, rtstarts, rtends,self.resolution])
+
+        #get EICs
+        result = startConcurrentTask(PeakDetective.getNormalizedIntensityVector, args, self.numCores, "forming matrix", len(args))
+
+        #concatenate EICs
+        result = np.concatenate(result,axis=0)
+
+        #align EICs
+        if align:
+            result = alignDataMatrix(result,featInds,True,self.numCores)
+
+        return result
+
+    def trainSmoother(self,peaks,raw_datas,numPeaks,smooth_epochs,batch_size,validation_split):
+        """
+        Train smoothing autoencoder network
+        @param peaks: Pandas DataFrame, list of features detected from some peak detection software
+        @param raw_datas: list of rawData objects, samples to use for training
+        @param numPeaks: int, number of peaks to sample to train autoencoder
+        @param smooth_epochs: int, number of epochs to train for
+        @param batch_size: int, batch size for training
+        @param validation_split: float, fraction of EICs to hold out for validation, between 0-1.
+        @return: None
+        """
+        #generate data matrix
+        print("generating EICs...")
+        mzs = rd.choices(list(peaks["mz"].values),k=int(numPeaks/len(raw_datas)))
+        rts = rd.choices(list(peaks["rt"].values),k=int(numPeaks/len(raw_datas)))
+
+        X = self.makeDataMatrix(raw_datas,mzs,rts)
+
+        #normalize matrix
+        X_norm = normalizeMatrix(X)
+
+        print("done")
+
+        #fit autoencoder
+        print("fitting smoother...")
+        smoother = Smoother(self.resolution)
+        smoother.fit(X_norm, X_norm, epochs=smooth_epochs, batch_size=batch_size, validation_split=validation_split,verbose=1)
+
+        #set updated models
+        self.smoother = smoother
+        self.encoder = keras.Model(smoother.input, smoother.layers[7].output)
+        print("done")
+
+    def trainClassifier(self,X,y,X_val,y_val,min_epochs,max_epochs,batch_size,restarts):
+        """
+        Train classifer network
+        @param X: numpy matrix, input EICs to train on
+        @param y: numpy matrix, input labels to train on
+        @param X_val: numpy matrix, EICs to use a validation data
+        @param y_val: numpy matrix, input labels to use as validation
+        @param min_epochs: int, minimum number of epochs to train
+        @param max_epochs: int, maximum number of epochs to train
+        @param batch_size: int, batch size to use when training
+        @param restarts: int, number of random restarts to run
+        @return: EarlyStopping callback, training history in keras callback object
+        """
+
+        #normalize matrix
+        X_norm = normalizeMatrix(X)
+
+        #calculate peak areas
+        tics = np.log10(np.array([np.max([2, integratePeak(x)]) for x in X]))
+
+        #get latent rep. of EICs
+        X_latent = self.encoder.predict(X_norm)
+
+        #normalize validation EICs
+        X_tmp = normalizeMatrix(X_val)
+
+        #get peak areas for validation data
+        tic_val = np.log10(np.array([np.max([2, integratePeak(x)]) for x in X_val]))
+
+        #get latent rep. of validaiton EICs
+        X_val = self.encoder.predict(X_tmp)
+
+
+        #begin training
+        bestLoss = np.inf
+        bestWeights = -1
+        bestValErr = -1
+        bestBestEpoch = -1
+        trainErr = -1
+        trainLoss = -1
+
+        #iterate over random restarts
+        for x in range(restarts):
+
+            #make callback object
+            cb = keras.callbacks.EarlyStopping(
+                monitor="val_loss",
+                min_delta=0,
+                patience=3,
+                verbose=0,
+                mode="auto",
+                baseline=None,
+                restore_best_weights=True,
+            )
+
+            history = keras.callbacks.History()
+
+            # initialize classifier
+            classifer = ClassifierLatent(X_latent.shape[1])
+
+            #train to minimum epochs
+            if min_epochs > 0:
+                classifer.fit([X_latent,tics],y,epochs=int(min_epochs),batch_size=batch_size,verbose=0,
+                              validation_data=([X_val, tic_val], y_val))
+
+            #train until maximum epochs with early stopping
+            classifer.fit([X_latent, tics], y, epochs=int(max_epochs-min_epochs),
+                          batch_size=batch_size, verbose=0, callbacks=[cb, history],
+                          validation_data=([X_val, tic_val], y_val))
+
+            #get performance
+            valLoss = history.history["val_loss"][cb.best_epoch]
+            valErr = history.history["val_mean_absolute_error"][cb.best_epoch]
+            bestEpoch = cb.best_epoch
+
+            #update best performers
+            if valLoss < bestLoss:
+                bestLoss = valLoss
+                bestWeights = classifer.get_weights()
+                bestValErr = valErr
+                bestBestEpoch = bestEpoch
+                trainLoss = history.history["loss"][cb.best_epoch]
+                trainErr = history.history["mean_absolute_error"][cb.best_epoch]
+
+        #print performance
+        print("loss:",trainLoss,"mean_absolute_error:",trainErr,"val loss:", bestLoss, "val_mean_absolute_error:",bestValErr, "numEpochs:", min_epochs + bestBestEpoch)
+
+        #set best weights
+        classifer.set_weights(bestWeights)
+
+        self.classifier = classifer
+
+        return history
+
+    def trainClassifierActive(self,X,X_labeled,y_labeled,min_epochs,max_epochs,batch_size,restarts,numVal = 10,numManualPerRound=3,inJupyter=True):
+        trainingInds = []
+
+        valInds = list(range(len(X)))
+        valInds = rd.sample(valInds,numVal)
+
+        y = np.zeros((len(X)-numVal,2))
+
+        X_val = X[valInds]
+        y_val = np.zeros((numVal,2))
+
+        X = X[[x for x in range(len(X)) if x not in valInds]]
+
+        updatingInds = list(range(len(X)))
+
+        for ind in range(len(X_val)):
+            val = self.labelPeak([X_val[ind]], -1*self.windowSize/2, self.windowSize/2, inJupyter,"","relative retention time")
+            y_val[ind, 0] = 1 - val
+            y_val[ind, 1] = val
+
+
+        if len(X_labeled) > 0:
+            self.trainClassifier(X_labeled,
+                                 y_labeled,
+                                 X_val,y_val, min_epochs,max_epochs, batch_size, restarts)
+
+        y[updatingInds] = self.classifyMatrix(X[updatingInds])
+
+        doMore = True
+        i=0
+
+        def padVal(val):
+            if val < 0.5:
+                return val + 1e-8
+            else:
+                return val - 1e-8
+
+        while doMore:
+            if len(updatingInds) > 0:
+
+                entropies = [-1 * np.sum([padVal(val) * np.log(padVal(val)) for yyy in yy]) for yy in y[updatingInds]]
+
+                order = list(range(len(updatingInds)))
+                order.sort(key=lambda x: entropies[x], reverse=True)
+                order = [updatingInds[x] for x in order]
+
+                if len(order) < numManualPerRound:
+                    numManualPerRound = len(order)
+
+                inds = np.random.choice(order,numManualPerRound,replace=False,p=np.array(entropies) / np.sum(entropies))
+
+                #inds = order[:numManualPerRound]
+
+                for ind in inds:
+                    val = self.labelPeak([X[ind]], -1*self.windowSize/2, self.windowSize/2, inJupyter, y[ind][1],"relative retention time")
+                    y[ind, 0] = 1 - val
+                    y[ind, 1] = val
+                    trainingInds.append(ind)
+                    updatingInds.remove(ind)
+
+                if len(X_labeled) > 0:
+                    X_train = np.concatenate((X[trainingInds],X_labeled),axis=0)
+                    y_train = np.concatenate((y[trainingInds],y_labeled),axis=0)
+                else:
+                    X_train = X[trainingInds]
+                    y_train = y[trainingInds]
+
+                if len(X_train) > 0:
+                    self.trainClassifier(X_train,y_train,X_val,y_val,min_epochs,max_epochs,batch_size,restarts)
+
+                y[updatingInds] = self.classifyMatrix(X[updatingInds])
+
+                plt.figure()
+                plt.hist(y[:, 1], bins=20)
+                plt.title("round" + str(i + 1))
+                plt.xlabel("PeakDetective Score")
+                plt.ylabel("Number of features")
+                plt.show()
+
+                print(str(len(updatingInds)) + " unclassified features remaining")
+                print("Continue with another iteration? (1=Yes, 0=No): ")
+                tmp = float(input())
+                while not validateInput(tmp):
+                    print("invalid classification: ")
+                    tmp = float(input())
+                doMore = bool(tmp)
+
+            else:
+                doMore = False
+            i += 1
+
+        plotScoringStatistics(self.classifyMatrix(X_val)[:,1],y_val[:,1])
+
+
+    def classifyMatrix(self,X):
+        # normalize matrix
+        X_norm = normalizeMatrix(X)
+        peak_areas = np.log10(np.array([np.max([2, integratePeak(x)]) for x in X]))
+
+        X_latent = self.encoder.predict(X_norm)
+        y = self.classifier.predict([X_latent, peak_areas])
+        return y
+
+
+
+    def detectPeaksTargeted(self,raw_datas,peaks,ppmCutoff=10,rtCutoff=0.5,cutoff=0.5, intensityCutoff = 100,window=0.05,align=True,detectFrac=0.0,isotope="M+0"):
+
+        #find peaks in targeted list
+        rois = peaks[peaks["isotope"] == isotope]["mz"].values
+
+        peak_scores,peak_intensities = self.detectPeaksFromROIs(raw_datas,rois, cutoff, intensityCutoff,window,align,detectFrac)
+
+        #look for closest match
+        founds = []
+        mzs = []
+        rts = []
+        for index,row in peaks.iterrows():
+            if row["isotope"] == isotope:
+                filt = peak_scores[(peak_scores["rt"] > row["rt"] - rtCutoff) & (peak_scores["rt"] < row["rt"] + rtCutoff)]
+                if len(filt) > 0:
+                    minMz = row["mz"] - ppmCutoff/1e6 * row["mz"]
+                    maxMz = row["mz"] + ppmCutoff/1e6 * row["mz"]
+                    filt = filt[(filt["mz"] > minMz) & (filt["mz"] < maxMz)]
+                    if len(filt) > 0:
+                        filt["rt_diff"] = [np.abs(row["rt"] - rt) for rt in filt["rt"]]
+                        filt["ppm_error"] = [1e6 * np.abs(row["mz"] - mz)/row["mz"] for mz in filt["mz"]]
+                        filt = filt.sort_values(by="rt_diff",ascending=True)
+
+                        mzError = filt["mz"].values[0] - row["mz"]
+
+                        peaks_filt = peaks[peaks["group"] == row["group"]]
+
+                        for index2,row2 in peaks_filt.iterrows():
+                            founds.append(index2)
+                            mzs.append(row2["mz"] + mzError)
+                            rts.append(filt["rt"].values[0])
+
+
+        peaks = peaks.loc[founds,:]
+        peaks["mz_searched"] = peaks["mz"]
+        peaks["rt_searched"] = peaks["rt"]
+        peaks["mz"] = mzs
+        peaks["rt"] = rts
+
+        X = self.makeDataMatrix(raw_datas, mzs, rts, align=align)
+
+        y = self.classifyMatrix(X)
+
+        peak_curated = deepcopy(peaks)
+        peak_scores = deepcopy(peaks)
+        peak_intensities = deepcopy(peaks)
+
+        keys = []
+        for raw in raw_datas:
+            peak_scores[raw.filename] = np.zeros(len(peak_scores.index.values))
+            peak_intensities[raw.filename] = np.zeros(len(peak_scores.index.values))
+            for index in peaks.index.values:
+                keys.append([raw.filename, index])
+
+        for [file, index], score in zip(keys, y[:, 1]):
+            peak_scores.at[index, file] = score
+            val = 0
+            if score > cutoff:
+                val = 1
+            peak_curated.at[index, file] = val
+
+        if "peak_group" in peaks.columns.values:
+            peak_groups = peaks[["peak_group"]]
+        else:
+            peak_groups = None
+
+        peak_intensities = self.performIntegration(X, [raw.filename for raw in raw_datas], peak_scores, cutoff,peakGrouping=peak_groups)
+
+        return peaks, peak_curated, peak_scores, peak_intensities
+
+    def detectPeaksFromROIs(self, rawDatas, rois, cutoff=0.5, intensityCutoff = 100,window=0.05,align=True,detectFrac=0.0):
+        print("generating all EICs from ROIs...")
+        dt = self.windowSize / self.resolution
+        tmpRes = int(math.ceil((rawDatas[0].rts[-1] - rawDatas[0].rts[0] + self.windowSize) / dt))
+        oldRes = int(self.resolution)
+        oldwindow = float(self.windowSize)
+        self.resolution = tmpRes
+        self.windowSize = rawDatas[0].rts[-1] + self.windowSize / 2 - rawDatas[0].rts[0] + self.windowSize / 2
+        rts = [(rawDatas[0].rts[-1] + rawDatas[0].rts[0]) / 2 for _ in rois]
+        X_tot = self.makeDataMatrix(rawDatas, rois, rts, align)
+        self.resolution = oldRes
+        self.windowSize = oldwindow
+
+        numPoints = 0
+        rt = rawDatas[0].rts[0]
+        while (rt <= rawDatas[0].rts[-1]):
+            numPoints += 1
+            rt += window
+
+        X = np.zeros((int(numPoints * len(rois) * len(rawDatas)), self.resolution))
+
+        mzs = []
+        rts = []
+        files = []
+        featInds = []
+
+        counter = 0
+        rowCounter = 0
+        trueDt = tmpRes / (rawDatas[0].rts[-1] + self.windowSize / 2 - rawDatas[0].rts[0] + self.windowSize / 2)
+        stride = int(np.floor(window * trueDt))
+
+        for rawData in rawDatas:
+            i = 0
+            for row in range(len(rois)):
+                rt = float(rawDatas[0].rts[0])
+                start = 0
+                end = start + self.resolution
+                for _ in range(numPoints):
+                    if end >= X_tot.shape[1]:
+                        n = X_tot.shape[1] - start
+                        print(start, end, n, X.shape, X_tot.shape, numPoints)
+                        X[counter, :n] = X_tot[rowCounter, start:]
+                    else:
+                        X[counter, :] = X_tot[rowCounter, start:end]
+                    counter += 1
+                    start += stride
+                    end += stride
+                    mzs.append(rois[row])
+                    rts.append(rt)
+                    rt += window
+                    files.append(rawData.filename)
+                    featInds.append(i)
+                    i += 1
+                rowCounter += 1
+
+        X = X[:counter]
+
+        print(len(X), "EICs constructed for evaluation")
+
+        peak_areas = [integratePeak(x) for x in X]
+        toClassify = [x for x in range(len(peak_areas)) if peak_areas[x] > intensityCutoff]
+
+        peak_scores = pd.DataFrame(index=range(len(set(featInds))))
+
+        orderedMzs = []
+        orderedRts = []
+
+        for row in range(len(rois)):
+            rt = float(rawDatas[0].rts[0])
+            for _ in range(numPoints):
+                orderedMzs.append(rois[row])
+                orderedRts.append(rt)
+                rt += window
+
+        peak_scores["mz"] = orderedMzs
+        peak_scores["rt"] = orderedRts
+
+        for rawData in rawDatas:
+            peak_scores[rawData.filename] = 0.0
+
+        y = np.zeros(len(X))
+        y[toClassify] = self.classifyMatrix(X[toClassify])[:, 1]
+        print("done")
+
+        goodInds = []
+        for id, filename, score in zip(featInds, files, y):
+            if score > cutoff:
+                goodInds.append(id)
+            peak_scores.at[id, filename] = score
+
+        detectNum = int(np.ceil(len(rawDatas) * detectFrac))
+        counts = {x: 0 for x in list(set(goodInds))}
+        for x in goodInds:
+            counts[x] += 1
+        goodInds = [x for x in counts if counts[x] >= detectNum]
+        goodInds.sort()
+
+        toKeep = []
+        for x in range(len(rawDatas)):
+            for g in goodInds:
+                toKeep.append(x * len(peak_scores) + g)
+
+        X = X[toKeep]
+
+        peak_scores = peak_scores.loc[goodInds, :]
+
+        peak_scores = peak_scores.reset_index()
+
+        apex_rts = self.updateRT(peak_scores, [raw.filename for raw in rawDatas], X, cutoff)
+
+        peak_scores["rt"] = np.round(apex_rts, 2)
+
+        apex_mzs = self.updateMz(peak_scores, rawDatas, cutoff)
+
+        peak_scores["mz"] = np.round(apex_mzs, 7)
+
+        peak_intensities = self.performIntegration(X, [raw.filename for raw in rawDatas], peak_scores, cutoff)
+
+        peak_intensities = peak_intensities.drop_duplicates(["mz", "rt"], keep="first")
+        peak_scores = peak_scores.drop_duplicates(["mz", "rt"], keep="first")
+
+        print(len(peak_scores), " peaks found")
+
+        return peak_scores, peak_intensities
+
+    def curatePeaks(self,raw_datas,peaks,threshold=0.5,align=False):
+        print("generating EICs...")
+        mzs = peaks["mz"].values
+        rts =  peaks["rt"].values
+
+        X = self.makeDataMatrix(raw_datas,mzs,rts,align=align)
+
+        y = self.classifyMatrix(X)
+
+        peak_curated = deepcopy(peaks)
+        peak_scores = deepcopy(peaks)
+        peak_intensities = deepcopy(peaks)
+
+        keys = []
+        for raw in raw_datas:
+            peak_scores[raw.filename] = np.zeros(len(peak_scores.index.values))
+            peak_intensities[raw.filename] = np.zeros(len(peak_scores.index.values))
+            for index in peaks.index.values:
+                keys.append([raw.filename, index])
+
+        for [file, index], score in zip(keys, y[:, 1]):
+            peak_scores.at[index, file] = score
+            val = 0
+            if score > threshold:
+                val = 1
+            peak_curated.at[index, file] = val
+
+        peak_intensities = self.performIntegration(X, [raw.filename for raw in raw_datas], peak_scores, threshold)
+
+        return peak_curated,peak_scores,peak_intensities
+
+    def detectPeaks(self, rawDatas, cutoff=0.5, intensityCutoff = 100,numDataPoints=3,window=0.05,align=True,detectFrac=0.0):
+        rois = self.roiDetection(rawDatas, intensityCutoff=intensityCutoff, numDataPoints=numDataPoints)
+        peak_scores,peak_intensities = self.detectPeaksFromROIs(rawDatas,rois, cutoff, intensityCutoff ,window,align,detectFrac)
+        return peak_scores,peak_intensities,rois
+
+    def updateRT(self,peakScores,samples,X,cutoff,smooth=False):
+        i = 0
+        rts = []
+        dt = self.windowSize / self.resolution
+        for index, row in peakScores.iterrows():
+            inds = []
+            allInds = []
+            for n,samp in enumerate(samples):
+                ind = i + n * len(peakScores)
+                if row[samp] > cutoff:
+                    inds.append(ind)
+                allInds.append(ind)
+            if len(inds) > 0:
+                tmp = X[inds].sum(axis=0)
+                if smooth: tmp = self.smoother.predict(normalizeMatrix(np.array([tmp])), verbose=0)[0]
+                lb, rb, apex = findPeakBoundaries(tmp)
+
+            else:
+                apex = (self.resolution-1)/2
+
+            rt = (apex - (self.resolution-1)/2) * dt + row["rt"]
+            rts.append(rt)
+            i += 1
+            printProgressBar(i, len(peakScores), "refining retention times", printEnd="")
+
+        return rts
+
+    def updateMz(self,peak_scores,raw_data,cutoff):
+        mzs = []
+        i = 0
+        for index,row in peak_scores.iterrows():
+            tmp = []
+            for data in raw_data:
+                if row[data.filename] > cutoff:
+                    tmp.append(data.getApexMz(row["mz"],row["rt"]))
+            tmp = np.array(tmp)
+            mzs.append(np.average(tmp[:,0],weights=tmp[:,1]))
+            i += 1
+            printProgressBar(i, len(peak_scores), "refining mzs", printEnd="")
+        return mzs
+
+    def label_peaks(self,raw_data,peaks,inJupyter = True):
+        rt_starts = [row["rt"] - self.windowSize/2 for _,row in peaks.iterrows()]
+        rt_ends = [row["rt"] + self.windowSize/2 for _,row in peaks.iterrows()]
+        y = []
+        mat = self.makeDataMatrix([raw_data],peaks["mz"].values,peaks['rt'])
+        count = 1
+        for vec,rt_start,rt_end in zip(mat,rt_starts,rt_ends):
+            y.append(self.labelPeak([vec],rt_start,rt_end,inJupyter,str(count) + "/" + str(len(mat)),"retention time"))
+            count += 1
+        peaks["classification"] = y
+        return peaks
+
+    def labelPeak(self,vecs,rt_start,rt_end,inJupyter,title="",xlabel="retention time"):
+        plt.figure()
+        plt.ion()
+        xs = np.linspace(rt_start, rt_end, len(vecs[0]))
+        [plt.plot(xs, vec) for vec in vecs]
+        plt.xlabel(xlabel)
+        plt.ylabel("intensity")
+        plt.title(title)
+        plt.show(block=False)
+        plt.pause(0.001)
+        print("Enter classification (1=True Peak, 0=Artifact): ")
+        val = input()
+
+        while not validateInput(val):
+            print("invalid classification: ")
+            val = input()
+        val = float(val)
+        plt.close()
+        if inJupyter:
+            IPython.display.clear_output(wait=True)
+
+        return val
+
+    def roiDetection(self,rawdatas,intensityCutoff=100,numDataPoints = 3):
+        rtss = [rawdata.rts for rawdata in rawdatas]
+        rois = []
+
+        counter = 0
+        totalNum = np.sum([len(rts) for rts in rtss])
+        for rts,rawdata in zip(rtss,rawdatas):
+            ppm = rawdata.ppm
+            for rt in rts:
+                printProgressBar(counter, totalNum,prefix = "Detecting ROIs",suffix=str(len(rois)) + " ROIs found",printEnd="")
+                counter += 1
+                for mz, i in rawdata.data[rt]:
+                    if i > intensityCutoff:
+                        update,pos = binarySearchROI(rois,mz,ppm)
+                        if update:
+                            rois[pos]["mzs"].append(mz)
+                            rois[pos]["mz_mean"] = np.mean(rois[pos]["mzs"])
+                            rois[pos]["extended"] = True
+                            rois[pos]["count"] += 1
+                        else:
+                            if pos != len(rois):
+                                rois.insert(pos,{"mz_mean":mz,"mzs":[mz],"extended":True,"count":1})
+                            else:
+                                rois.append({"mz_mean":mz,"mzs":[mz],"extended":True,"count":1})
+
+            toKeep = []
+            for x in range(len(rois)):
+                if rois[x]["extended"] == True or rois[x]["count"] >= numDataPoints:
+                    toKeep.append(x)
+
+            rois = [rois[x] for x in toKeep]
+
+            for x in range(len(rois)):
+                rois[x]["extended"] = False
+
+
+        rois = [x["mz_mean"] for x in rois]
+        print()
+        print(len(rois)," ROIs found")
+
+        return rois
+
+    def filterPeakListByScores(self,peakScores,samples,cutoff,frac):
+        goodInds = [index for index,row in peakScores.iterrows() if float(len([x for x in samples if row[x] > cutoff])) / len(samples) > frac]
+        return peakScores.loc[goodInds,:]
+
+    def performIntegration(self, X, samples, peakScores, cutoff, defaultWidth=0.5,smooth=False,peakGrouping=None):
+
+        if peakGrouping is None:
+            peakGrouping = pd.DataFrame(index=peakScores.index.values)
+            peakGrouping["peak_group"] = [x for x in range(len(peakGrouping))]
+
+        mapper = {index:i for index,i in zip(peakScores.index.values,range(len(peakScores)))}
+
+        peak_areas = pd.DataFrame(index=peakScores.index.values,columns=["mz","rt"])
+        peak_areas["mz"] = peakScores["mz"].values
+        peak_areas["rt"] = peakScores["rt"].values
+        peak_areas[samples] = np.zeros(peakScores[samples].values.shape)
+        print("integrating peaks...")
+
+        integ_groups = list(set(peakGrouping["peak_group"].values))
+        counter = 0
+        for g in integ_groups:
+            filt = peakScores.loc[peakGrouping[peakGrouping["peak_group"] == g].index.values,:]
+            inds = []
+            allInds = []
+            sampList = []
+            for index,row in filt.iterrows():
+                i = mapper[index]
+                for n, samp in enumerate(samples):
+                    ind = i + n * len(peakScores)
+                    if row[samp] > cutoff:
+                        inds.append(ind)
+                    allInds.append(ind)
+                    sampList.append(samp)
+            if len(inds) > 0:
+                tmp = X[inds].sum(axis=0)
+                if smooth: tmp = self.smoother.predict(normalizeMatrix(np.array([tmp])),verbose=0)[0]
+                lb,rb,apex = findPeakBoundaries(tmp)
+            else:
+                lb = int(np.round(self.resolution / 2 - defaultWidth * self.resolution / 2))
+                rb = int(np.round(self.resolution/2 + defaultWidth * self.resolution/2))
+            for ind,sample in zip(allInds,sampList):
+                peak_areas.at[index,sample] = integratePeak(X[ind],[lb,rb])
+            counter += 1
+            printProgressBar(counter, len(integ_groups), "integrating peaks", printEnd="")
+
+        return peak_areas
+
+
+class rawData():
+    def __init__(self,data={},filename="",ppm=0,timestamp=None):
+        self.data = data
+        self.filename = filename
+        self.rts = list(self.data.keys())
+        self.rts.sort()
+        self.ppm = ppm
+        self.timestamp = None
+
+    def readRawDataFile(self,filename,ppm,intensityThresh = 0):
+        """
+         Read MS datafile
+
+        :param filename: str, path to MS datafile
+        """
+        try:
+            try:
+                with mzml.MzML(filename.replace('"', "")) as f:
+                    self.timestamp = datetime.datetime.fromisoformat(next(f.iterfind('run', recursive=False))['startTimeStamp'][:-1]).astimezone(datetime.timezone.utc)
+            except:
+                print("Warning: file timestamp could not be read")
+                self.timestamp = None
+            reader = mzml.read(filename.replace('"', ""))
+            ms1Scans = {}
+            for temp in reader:
+                if temp['ms level'] == 1:
+                    spectrum = [[mz,i] for mz, i in zip(temp["m/z array"],temp["intensity array"]) if i > intensityThresh]
+                    spectrum.sort(key=lambda x:x[0])
+                    ms1Scans[temp["scanList"]["scan"][0]["scan start time"]] = spectrum
+            reader.close()
+            self.rts = list(ms1Scans.keys())
+            self.rts.sort()
+            self.data = ms1Scans
+            self.filename = filename
+            self.ppm = ppm
+
+        except:
+            print(sys.exc_info())
+            print(filename + " does not exist or is ill-formatted")
+
+
+    def extractEIC(self,mz,rt_start,rt_end):
+        width = self.ppm * mz / 1e6
+        mz_start = mz - width
+        mz_end = mz + width
+        rts = [x for x in self.rts if x > rt_start and x < rt_end]
+        intensity = []
+        for rt in rts:
+            Origind = getIndexOfClosestValue([x[0] for x in self.data[rt]],mz)
+            ind = int(Origind)
+            tmp = 0
+            while  ind < len(self.data[rt]) and self.data[rt][ind][0] > mz_start and self.data[rt][ind][0] < mz_end:
+                tmp += self.data[rt][ind][1]
+                ind += 1
+            ind = Origind - 1
+            while ind > -1 and self.data[rt][ind][0] > mz_start and self.data[rt][ind][0] < mz_end :
+                tmp += self.data[rt][ind][1]
+                ind -= 1
+            intensity.append(tmp)
+        return rts,intensity
+
+    def getApexMz(self,mz,rt):
+        width = self.ppm * mz / 1e6
+        mz_start = mz - width
+        mz_end = mz + width
+        rt = self.rts[getIndexOfClosestValue(self.rts,rt)]
+        highestMz = mz
+        highestIntensity = 1
+        Origind = getIndexOfClosestValue([x[0] for x in self.data[rt]], mz)
+        ind = int(Origind)
+        while ind < len(self.data[rt]) and self.data[rt][ind][0] > mz_start and self.data[rt][ind][0] < mz_end:
+            if self.data[rt][ind][1] > highestIntensity:
+                highestIntensity = self.data[rt][ind][1]
+                highestMz = self.data[rt][ind][0]
+            ind += 1
+        ind = Origind - 1
+        while ind > -1 and self.data[rt][ind][0] > mz_start and self.data[rt][ind][0] < mz_end:
+            if self.data[rt][ind][1] > highestIntensity:
+                highestIntensity = self.data[rt][ind][1]
+                highestMz = self.data[rt][ind][0]
+            ind -= 1
+        return highestMz,highestIntensity
+
+    def interpolate_data(self,mz,rt_start,rt_end):
+        rts,intensity = self.extractEIC(mz,rt_start,rt_end)
+        if len(rts) > 3:
+            #smoothing = smoothing * len(rts) * np.max(intensity)
+            #s = UnivariateSpline(rts,intensity,ext=1,s=smoothing)
+            s = interp1d(rts,intensity,kind="linear",fill_value=0,bounds_error=False)
+        else:
+            #s = UnivariateSpline([0,5,10,15],[0,0,0,0],ext=1,s=smoothing)
+            s = interp1d([0,5,10,15],[0,0,0,0],kind="linear",fill_value=0,bounds_error=False)
+
+        return s
+
+    def getMergedSpectrum(self,rtRange=None,intensityThresh=0,ppm=1):
+        if rtRange is None:
+            rtRange = [self.rts[0],self.rts[-1]]
+        spectra = [[[mz,i] for mz,i in self.data[rt] if i > intensityThresh] for rt in self.rts if rt > rtRange[0] and rt < rtRange[1]]
+        return mergeSpectra(spectra,ppm)
+
+
+def Smoother(resolution):
+    # build autoencoder
+    autoencoderInput = keras.Input(shape=(resolution,))
+    x = layers.Reshape((resolution, 1))(autoencoderInput)
+
+    kernelsize = 3
+    stride = 1
+    max_norm_value = 2.0
+
+    x = layers.Conv1D(32, kernelsize, strides=stride, activation='relu', kernel_constraint=max_norm(max_norm_value),
+                     kernel_initializer='he_uniform')(x)
+
+    #x = layers.BatchNormalization()(x)
+
+    x = layers.Conv1D(16, kernelsize, strides=stride, activation='relu', kernel_constraint=max_norm(max_norm_value),
+                     kernel_initializer='he_uniform')(x)
+
+    #x = layers.BatchNormalization()(x)
+
+    x = layers.Conv1D(8, kernelsize, strides=stride, activation='relu', kernel_constraint=max_norm(max_norm_value),
+                      kernel_initializer='he_uniform')(x)
+
+    #x = layers.BatchNormalization()(x)
+
+    x = layers.Conv1D(4, kernelsize, strides=stride, activation='relu', kernel_constraint=max_norm(max_norm_value),
+                      kernel_initializer='he_uniform')(x)
+
+    #x = layers.BatchNormalization()(x)
+
+    x = layers.Flatten()(x)
+
+    x = layers.Dense(5, activation="relu")(x)
+
+    x = layers.Dense(int((resolution-8) * 4), activation="relu")(x)
+
+    x = layers.Reshape((resolution-8, 4))(x)
+
+    x = layers.Conv1DTranspose(8, kernelsize, strides=stride, activation='relu',
+                               kernel_constraint=max_norm(max_norm_value), kernel_initializer='he_uniform')(x)
+
+    #x = layers.BatchNormalization()(x)
+
+    x = layers.Conv1DTranspose(16, kernelsize, strides=stride, activation='relu',
+                              kernel_constraint=max_norm(max_norm_value), kernel_initializer='he_uniform')(x)
+
+    #x = layers.BatchNormalization()(x)
+
+    x = layers.Conv1DTranspose(32, kernelsize, strides=stride, activation='relu',
+                              kernel_constraint=max_norm(max_norm_value), kernel_initializer='he_uniform')(x)
+
+    #x = layers.BatchNormalization()(x)
+
+    x = layers.Conv1DTranspose(1, kernelsize, strides=stride, activation='sigmoid',
+                               kernel_constraint=max_norm(max_norm_value), kernel_initializer='he_uniform')(x)
+
+    x = layers.Flatten()(x)
+
+    autoencoder = keras.Model(autoencoderInput, x)
+
+    autoencoder.compile(loss='binary_crossentropy', optimizer=keras.optimizers.Adam(1e-4),
+                        metrics=['mean_absolute_error'],weighted_metrics=[])
+
+
+    return autoencoder
+
+def ClassifierLatent(resolution):
+    descriminatorInput = keras.Input(shape=(resolution,))
+    ticInput = keras.Input(shape=(1,))
+
+    #x = layers.Dense(resolution, activation="relu")(descriminatorInput)
+
+    x = layers.Layer()(descriminatorInput)
+
+    x = keras.Model(descriminatorInput, x)
+
+    tic = keras.Model(ticInput, layers.Layer()(ticInput))
+
+    x = layers.concatenate([x.output, tic.output], axis=1)
+
+    x = layers.Dense(int(resolution), activation="relu")(x)
+
+    x = layers.Dense(int(resolution), activation="relu")(x)
+
+    x = layers.Dense(int(resolution), activation="relu")(x)
+
+    x = layers.Dense(int(resolution), activation="relu")(x)
+
+    x = layers.Dense(int(resolution), activation="relu")(x)
+
+    output = layers.Dense(2, activation="softmax")(x)
+
+    classifier = keras.Model([descriminatorInput, ticInput], output, name="discriminator")
+
+    classifier.compile(loss='binary_crossentropy', optimizer=keras.optimizers.Adam(1e-4),
+                          metrics=['mean_absolute_error'])
+
+    return classifier
+
+
+def makePRCPlot(pred,true,noSkill=True):
+
+    prec, recall, threshs = met.precision_recall_curve(true, pred)
+
+    auc = np.round(met.auc(recall, prec), 4)
+
+    plt.plot(recall, prec, label="prAUC=" + str(auc))
+    plt.xlabel("Recall")
+    plt.ylabel("Precision")
+    if noSkill:
+        numPositive = len([x for x in true if x > 0.5])
+        numNegative = len(true) - numPositive
+        plt.plot([0, 1.0],
+                 [numPositive / float(numPositive + numNegative), numPositive / float(numPositive + numNegative)],
+                 label="NSL prAUC=" + str(
+                     np.round(numPositive / float(numPositive + numNegative), 4)))
+    plt.legend()
+    return auc
+
+
+def findPeakBoundaries(peak):
+    apex = int(len(peak)/2)
+    #find left bound
+
+    foundNewApex = True
+
+    while(foundNewApex):
+        foundNewApex = False
+
+        x = apex
+        while peak[x] > peak[apex] / 2 and x > 0:
+            if peak[x] > peak[apex]:
+                apex = x
+            x -= 1
+        lb = x
+
+        x = apex
+        while peak[x] > peak[apex] / 2 and x < len(peak) - 1:
+            if peak[x] > peak[apex]:
+                apex = x
+                foundNewApex = True
+            x += 1
+        rb = x
+
+    return lb,rb,apex
+
+def integratePeak(peak,bounds=None):
+    if bounds is None:
+        lb,rb,apex = findPeakBoundaries(peak)
+    else:
+        lb = bounds[0]
+        rb = bounds[1]
+    if lb != rb:
+        try:
+            area = np.trapz(peak[lb:rb],np.linspace(lb,rb,rb-lb))
+        except:
+            print(lb,rb)
+            area = 0
+    else:
+        area = 0
+    return area
+
+
+def alignPeaks(peaks,normalize=True,reference=0,q=None):
+    if normalize:
+        peaks_norm = [safeNormalize(x) for x in peaks]
+    else:
+        peaks_norm = deepcopy(peaks)
+
+    reference_peak = peaks_norm[reference]
+    ref = list(range(len(reference_peak)))
+
+    for x,peak in enumerate(peaks_norm):
+        if x > 0:
+            distance, path = fastdtw(np.array(reference_peak).flatten(), np.array(peak).flatten(), dist=2)
+            xs = []
+            ys = []
+
+            prev = path[0][0]
+            tmp = [peaks[x][path[0][1]]]
+            for p1,p2 in path[1:]:
+                if p1 != prev:
+                    xs.append(prev)
+                    ys.append(np.mean(tmp))
+                    tmp = []
+                tmp.append(peaks[x][p2])
+                prev = p1
+            xs.append(prev)
+            ys.append(np.mean(tmp))
+
+
+            f = interp1d(xs,ys,fill_value=0.0,bounds_error=False)
+            peaks[x] = [f(i) for i in ref]
+
+
+    if type(q) != type(None):
+        q.put(0)
+
+    return peaks
+
+def alignDataMatrix(matrix,peakInds,normalize=True,numCores=1):
+    uniquePeaks = list(set(peakInds))
+    order = [[] for _ in uniquePeaks]
+    args = [[[],normalize,0] for _ in uniquePeaks]
+    for i,peak,ind in zip(range(len(matrix)),matrix,peakInds):
+        args[ind][0].append(peak)
+        order[ind].append(i)
+    result = startConcurrentTask(alignPeaks,args,numCores,"aligning EICs",len(uniquePeaks))
+    for peaks,inds in zip(result,order):
+        for peak,ind in zip(peaks,inds):
+            matrix[ind] = peak
+    return matrix
+
+
+def takeClosestInd(myList, myNumber):
+    """
+    Assumes myList is sorted. Returns closest value to myNumber.
+
+    If two numbers are equally close, return the smallest number.
+    """
+
+    pos = bisect_left(myList, myNumber)
+    if pos == 0:
+        return pos
+    if pos == len(myList):
+        return len(myList) - 1
+    before = myList[pos - 1]
+    after = myList[pos]
+    if after - myNumber < myNumber - before:
+        return pos
+    else:
+        return pos-1
+
+def mergeSpectra(spectra,ppm):
+    if len(spectra) > 0:
+        mergedSpectrumMzs = [x[0] for x in spectra[0]]
+        mergedSpectrumInts = [x[1] for x in spectra[0]]
+
+        if len(spectra) > 1:
+            fact = ppm / 1e6
+            for spectrum in spectra[1:]:
+                for mz,i in spectrum:
+                    if len(mergedSpectrumMzs) > 0:
+
+                        x = takeClosestInd(mergedSpectrumMzs,mz)
+                        delta = mz * fact
+
+                        if mergedSpectrumMzs[x] > mz - delta and mergedSpectrumMzs[x] < mz + delta:
+                            mergedSpectrumInts[x] += i
+                        else:
+                            if mz < mergedSpectrumMzs[x]:
+                                mergedSpectrumMzs.insert(x,mz)
+                                mergedSpectrumInts.insert(x,i)
+                            else:
+                                mergedSpectrumMzs.insert(x+1,mz)
+                                mergedSpectrumInts.insert(x+1,i)
+
+                    else:
+                        mergedSpectrumMzs.append(mz)
+                        mergedSpectrumInts.append(i)
+    else:
+        mergedSpectrumMzs = []
+        mergedSpectrumInts = []
+
+
+    return [[mz,i] for mz,i in zip(mergedSpectrumMzs,mergedSpectrumInts)]
+
+#Utility functions:
+
+#runs a function concurently.
+def startConcurrentTask(task,args,numCores,message,total,chunksize="none",verbose=True):
+
+    if verbose:
+        m = Manager()
+        q = m.Queue()
+        args = [a + [q] for a in args]
+        t = Thread(target=updateProgress, args=(q, total, message))
+        t.start()
+    if numCores > 1:
+        p = Pool(numCores)
+        if chunksize == "none":
+            res = p.starmap(task, args)
+        else:
+            res = p.starmap(task, args, chunksize=chunksize)
+        p.close()
+        p.join()
+    else:
+        res = [task(*a) for a in args]
+    if verbose: t.join()
+    return res
+
+
+def safeNormalize(x):
+    """
+    Safely normalize a vector, x, to sum to 1.0. If x is the zero vector return the normalized unity vector
+    """
+    if np.sum(x) < 1e-6:
+        tmp = np.ones(x.shape)
+        return tmp / np.sum(tmp)
+    else:
+        return x/np.sum(x)
+
+def normalizeMatrix(X):
+    """
+    Normalize a matrix so that the rows of X sum to one
+    """
+    return np.array([safeNormalize(x) for x in X])
+
+def classify(preds):
+    """
+    Classify predictions, preds, by returning the index of the highest scoring class
+    """
+    classes = np.zeros(preds.shape)
+    for x in range(len(preds)):
+        classes[x,list(preds[x]).index(np.max(list(preds[x])))] = 1
+    return classes
+
+
+def take_closest(myList, myNumber):
+    """
+    Assumes myList is sorted. Returns closest value to myNumber.
+
+    If two numbers are equally close, return the smallest number.
+    """
+    pos = bisect_left(myList, myNumber)
+    if pos == 0:
+        return myList[0]
+    if pos == len(myList):
+        return myList[-1]
+    before = myList[pos - 1]
+    after = myList[pos]
+    if after - myNumber < myNumber - before:
+        return after
+    else:
+        return before
+
+
+
+def printProgressBar(iteration, total, prefix='', suffix='', decimals=1, length=50, fill='█', printEnd="\r"):
+    """
+    Call in a loop to create terminal progress bar
+    @params:
+        iteration   - Required  : current iteration (Int)
+        total       - Required  : total iterations (Int)
+        prefix      - Optional  : prefix string (Str)
+        suffix      - Optional  : suffix string (Str)
+        decimals    - Optional  : positive number of decimals in percent complete (Int)
+        length      - Optional  : character length of bar (Int)
+        fill        - Optional  : bar fill character (Str)
+        printEnd    - Optional  : end character (e.g. "\r", "\r\n") (Str)
+    """
+    percent = ("{0:." + str(decimals) + "f}").format(100 * (iteration / float(total)))
+    filledLength = int(length * iteration // total)
+    bar = fill * filledLength + '-' * (length - filledLength)
+    print(f'\r{prefix} |{bar}| {percent}% {suffix}', end=printEnd)
+    # Print New Line on Complete
+    if iteration == total:
+        print()
+
+def updateProgress(q, total,message = ""):
+    """
+    update progress bar
+    """
+    counter = 0
+    while counter != total:
+        if not q.empty():
+            q.get()
+            counter += 1
+            #if counter % 20 == 0:
+            printProgressBar(counter, total,prefix = message, printEnd="")
+
+
+def getIndexOfClosestValue(l,v):
+    """
+    get index of list with closest value to v, assumes l is sorted
+    """
+    pos = bisect_left(l, v)
+    if pos == 0:
+        return 0
+    if pos == len(l):
+        return pos - 1
+    before = l[pos - 1]
+    after = l[pos]
+    if after - v < v - before:
+        return pos
+    else:
+        return pos - 1
+
+def plotScoringStatistics(scores, labels):
+    tpr = []
+    fdr = []
+    cutoffs = np.linspace(0, 1.0, 100)
+    for cutoff in cutoffs:
+        fdr.append(1 - met.precision_score(labels, scores > cutoff, zero_division=0))
+        tpr.append(met.recall_score(labels, scores > cutoff, zero_division=0))
+    plt.scatter(cutoffs, tpr, c="black", label="TPR")
+    plt.plot(cutoffs, tpr, c="black")
+
+    plt.scatter(cutoffs, fdr, c="red", label="FDR")
+    plt.plot(cutoffs, fdr, c="red")
+    plt.legend()
+    plt.xlabel("cutoff")
+    plt.ylabel("performance")
+
+def validateInput(input):
+    """
+    Validate input, used for the labelPeaks() function
+    @param input: str, user input
+    @return: Bool, True = user input was a 0 or 1, False otherwise
+    """
+    try:
+        input = float(input)
+        if input not in [0, 1]:
+            return False
+        return True
+    except:
+        return False
+
+def binarySearchROI(poss, query, ppm):
+    """
+    Search function used in ROI calculations
+    """
+    if len(poss) == 0:
+        return False, 0
+
+    pos = bisect_left([x["mz_mean"] for x in poss], query)
+
+    if pos == len(poss):
+        if 1e6 * np.abs(query - poss[-1]["mz_mean"]) / query < ppm:
+            return True, pos - 1
+        else:
+            return False, pos
+    elif pos == 0:
+        if 1e6 * np.abs(query - poss[0]["mz_mean"]) / query < ppm:
+            return True, 0
+        else:
+            return False, pos
+    else:
+        ldiff = 1e6 * np.abs(query - poss[pos - 1]["mz_mean"]) / query
+        rdiff = 1e6 * np.abs(query - poss[pos]["mz_mean"]) / query
+
+        if ldiff < rdiff:
+            if ldiff < ppm:
+                return True, pos - 1
+            else:
+                return False, pos
+        else:
+            if rdiff < ppm:
+                return True, pos
+            else:
                 return False, pos
```

### Comparing `PeakDetective-0.1.6/PeakDetective/detection_helper.py` & `PeakDetective-0.1.8/PeakDetective/detection_helper.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,280 +1,280 @@
-import numpy as np
-import pandas as pd
-import scipy.stats as stats
-import os
-import uuid
-import bisect
-from . import printProgressBar, startConcurrentTask, getIndexOfClosestValue
-from sklearn.ensemble import RandomForestRegressor
-import matplotlib.pyplot as plt
-
-
-class PeakList():
-    def __init__(self,peakList = None):
-        if type(peakList) == type(None):
-            self.peakList = pd.DataFrame()
-        else:
-            self.peakList = peakList
-            
-    def from_df(self,df,sampleCols=None):
-        self.peakList = df
-        if sampleCols is None: self.sampleCols = [x for x in self.peakList.columns.values if x not in ["mz","rt","rt_start","rt_end","isotope","adduct","peak group"]]
-        else: self.sampleCols = sampleCols
-
-    def to_csv(self,fn):
-        self.peakList.to_csv(fn)
-
-    def to_skyline(self,fn,polarity,moleculeListName = "XCMS peaks"):
-        transitionList = pd.DataFrame(self.peakList)
-        transitionList["Precursor Name"] = ["unknown " + str(index) for index, row in transitionList.iterrows()]
-        transitionList["Explicit Retention Time"] = [row["rt_start"] / 2 + row["rt_end"] / 2 for index, row in
-                                                     transitionList.iterrows()]
-        polMapper = {"Positive": 1, "Negative": -1}
-        transitionList["Precursor Charge"] = [polMapper[polarity] for index, row in transitionList.iterrows()]
-        transitionList["Precursor m/z"] = [row["mz"] for index,row in transitionList.iterrows()]
-        transitionList["Molecule List Name"] = [moleculeListName for _ in range(len(transitionList))]
-        transitionList = transitionList[
-            ["Molecule List Name", "Precursor Name", "Precursor m/z", "Precursor Charge",
-             "Explicit Retention Time"]]
-        transitionList.to_csv(fn)
-
-
-
-    def readXCMSPeakList(self,filename,key=".mzML"):
-        data = pd.read_csv(filename,index_col=0,sep="\t")
-        data_form = {}
-        self.sampleCols = [x for x in data.columns.values if key in x]
-        for col in self.sampleCols:
-            data[col] = data[col].fillna(0)
-        for index,row in data.iterrows():
-            data_form[index] = {"mz":row["mzmed"],"rt":row["rtmed"]/60,"rt_start":row["rtmin"]/60,"rt_end":row["rtmax"]/60}#,"isotope_xcms":row["isotopes"],"adduct_xcms":row["adduct"],"peak group":row["pcgroup"]}
-            for col in self.sampleCols:
-               data_form[index][col] = row[col]
-               
-        self.peakList = pd.DataFrame.from_dict(data_form,orient="index")
-
-    def runXCMS(self, path, fn, polarity, ppm, peakWidth,noise=1000,s2n=1,prefilter = 2,mzDiff=0.0001,minFrac=0.0):
-        dir = os.path.dirname(__file__)
-        os.system("Rscript " + os.path.join(dir, "find_peaks.R") + " " + path + " " + polarity + " " + str(
-            ppm) + " " + str(peakWidth[0]) + " " + str(peakWidth[1]) + " " + fn + " " + str(noise) + " " + str(s2n) + " " + str(prefilter) + " " + str(mzDiff) + " " + str(minFrac))
-        self.readXCMSPeakList(path + fn)
-
-    def installRPackages(self):
-        dir = os.path.dirname(__file__)
-        os.system("Rscript " + os.path.join(dir, "install_R_packages.R"))
-
-    #def filterAdductsIsotopes(self,adductsToKeep = ["[M+H]","[M-H]"],isotopesToKeep = ["[M]"]):
-    #    goodRows = []
-    #    for index,row in self.peakList.iterrows():
-    #        if (pd.isna(row["adduct_xcms"]) or any(x in row["adduct_xcms"] for x in adductsToKeep)) and (pd.isna(row["isotope_xcms"]) or any(x in row["isotope_xcms"] for x in isotopesToKeep)):
-    #            goodRows.append(index)
-    #    self.peakList = self.peakList.loc[goodRows,:]
-
-    def removeRedundancy(self,corrThresh,rtThresh,polarity,ppm,numCores,sampleCols=None):
-
-        if sampleCols is None:
-            sampleCols = self.sampleCols
-
-        groups = []
-        anchors = []
-        rts = []
-        c = 0
-
-        self.peakList = self.peakList.sort_values(by="rt",ascending=True)
-        for index,row in self.peakList.iterrows():
-            unique = True
-            if len(rts) > 0:
-                iC = len(rts) - 1
-                rt, vec = anchors[iC]
-
-                if np.abs(rts[iC]-row["rt"]) < rtThresh:
-                    if len(sampleCols) > 2:
-                        r, p = stats.pearsonr(vec, row[sampleCols].values)
-                        if r > corrThresh:
-                            unique = False
-                            groups[iC].append(index)
-                    else:
-                        unique = False
-                        groups[iC].append(index)
-
-            if unique:
-                rts.append(row["rt"])
-                groups.append([index])
-                anchors.append([row["rt"],row[sampleCols].values])
-            c += 1
-            printProgressBar(c,len(self.peakList),prefix="grouping peaks",suffix=str(len(groups)) + " peak groups found",printEnd="")
-
-        self.peakList = self.peakList.sort_index()
-        args = []
-        for i,g in enumerate(groups):
-            filt = self.peakList.loc[g,:]
-            args.append([filt,polarity,ppm])
-        result = startConcurrentTask(runMzUnity,args,numCores,"running mz.unity",len(groups))
-        self.peakList["uniqueIon"] = True
-        for res,g in zip(result,groups):
-            self.peakList.loc[g,res.columns.values] = res.values
-
-        featsRemoved =  len(self.peakList) - len(self.peakList[self.peakList["uniqueIon"]])
-        self.peakList = self.peakList[self.peakList["uniqueIon"]]
-        print(featsRemoved,"redundant features found")
-
-    def backgroundSubtract(self,blank_keys,sample_keys,factor=3):
-        goodRows = []
-        sampleCols = [x for x in self.sampleCols if any(y in x for y  in sample_keys)]
-        blankCols = [x for x in self.sampleCols if any(y in x for y  in blank_keys) and x not in sampleCols]
-        for index,row in self.peakList.iterrows():
-            blankInt = np.mean(row[blankCols])
-            sampleInt = np.mean(row[sampleCols])
-            if sampleInt >= factor * blankInt:
-                goodRows.append(index)
-        print(len(self.peakList)-len(goodRows), "background features found")
-        self.peakList = self.peakList.loc[goodRows,:]
-
-    def imputeRowMin(self,sample_keys,minimum=1):
-
-        arr = self.peakList[sample_keys].values.transpose()
-
-        # find the minimum non-zero value of each compound
-        max_vals = []
-
-        for c in arr.transpose():
-            tmp = [x for x in c if x > minimum]
-            if len(tmp) > 0:
-                max_vals.append(np.min(tmp))
-            else:
-                max_vals.append(2)
-
-        # impute values
-        data_imp = np.zeros(arr.shape)
-        numImputted = 0
-        numNon = 0
-
-        for c in range(arr.shape[1]):
-            for r in range(arr.shape[0]):
-                # if not a missing value
-                if arr[r, c] > 1e-3:
-                    data_imp[r, c] = arr[r, c]
-                    numNon += 1
-                # if it is a missing value
-                else:
-                    data_imp[r, c] = max_vals[c] / 2
-                    numImputted += 1
-        print(numImputted / (numImputted + numNon), "of values imputted")
-
-
-        self.peakList[sample_keys] = data_imp.transpose()
-
-    def logTransform(self,sampleCols):
-        self.peakList[sampleCols] = np.log2(self.peakList[sampleCols].values)
-
-    def batchCorrect(self,sampleCols,qcCols,batchInfo,plot=True):
-
-        reg = RandomForestRegressor(n_jobs=10)
-
-        peak_areas = self.peakList[sampleCols].values.transpose()
-
-        X = np.array(batchInfo[qcCols])
-        y = peak_areas[qcCols] - np.mean(peak_areas[qcCols], axis=0)
-        reg.fit(X, y)
-        preds = reg.predict(batchInfo)
-        if plot:
-            plt.figure()
-            plt.plot(list(range(len(preds))),np.mean(preds,axis=1))
-            plt.errorbar(list(range(len(preds))),np.mean(preds,axis=1),yerr=np.std(preds,axis=1),fmt=".",capsize=1)
-            plt.xlabel("run order")
-            plt.ylabel("correction factor")
-        self.peakList[sampleCols] = np.array(peak_areas - preds).transpose()
-
-        
-
-def compareRT(feat1,feat2,rtTol):
-
-    rt1 = feat1["rt"]
-    rt2 = feat2["rt"]
-    
-    if np.abs(rt1-rt2) < rtTol:
-        return True
-        
-    return False
-
-def mergePeakLists(peakLists,names,ppm=20,rtTol=.5):
-    peakLists = [x[["mz","rt"]].reset_index() for x in peakLists]
-    mergedList = peakLists[0]
-    peakFounders = {n:{} for n in names}
-    peakIndices = {n:{} for n in names}
-
-    for index,row in mergedList.iterrows():
-        peakFounders[names[0]][index] = 1
-        peakIndices[names[0]][index] = index
-        for n in names[1:]:
-            peakFounders[n][index] = 0
-            peakIndices[n][index] = -1
-    for x,n in zip(peakLists[1:],names[1:]):
-        for index,row in x.iterrows():
-            new = True
-            mz_bounds = [row["mz"] - ppm*row["mz"]/1e6,row["mz"] + ppm*row["mz"]/1e6]
-            if len(mergedList) > 0:
-                filt = mergedList[(mergedList["mz"] > mz_bounds[0]) & (mergedList["mz"] < mz_bounds[1])]            
-                for index2,row2 in filt.iterrows():
-                    if compareRT(row,row2,rtTol):
-                        new = False
-                        peakFounders[n][index2] = 1
-                        peakIndices[n][index2] = index
-                        break
-            if new:
-                ind = len(mergedList)
-                mergedList = pd.concat((mergedList,x.iloc[index:index+1,:]),axis=0,ignore_index=True)
-                for n2 in names:
-                    peakFounders[n2][ind] = 0
-                    peakIndices[n2][ind] = -1
-
-                peakFounders[n][ind] = 1
-                peakIndices[n][ind] = index
-                
-      
-                            
-    peakFounders = pd.DataFrame.from_dict(peakFounders,orient="index").transpose()
-    peakIndices = pd.DataFrame.from_dict(peakIndices,orient="index").transpose()
-
-    return pd.concat((mergedList,peakFounders),axis=1,ignore_index=False),pd.concat((mergedList,peakIndices),axis=1,ignore_index=False)
-
-def runMzUnity(df,polarity,ppm,q=None):
-    dir = os.path.dirname(__file__)
-    path = str(uuid.uuid4()) + ".csv"
-    if len(df) > 1:
-        df.to_csv(path)
-        os.system("Rscript " + os.path.join(dir, "mz_unity.R") + " " + path + " " + str(polarity) + " " + str(ppm) + " " + path)
-        df = pd.read_csv(path,index_col=0)
-        if "uniqueIon" not in df.columns.values:
-            print("bad",len(df))
-            df["uniqueIon"] = True
-        else:
-            os.remove(path)
-
-    else:
-        df["uniqueIon"] = True
-
-    #check for duplicate mzs
-    mzs = df["mz"].values
-    for x in range(len(mzs)):
-        for y in range(x):
-            if abs(mzs[x] - mzs[y])/mzs[x] < ppm:
-                df.at[df.index.values[y],"uniqueIon"] = False
-
-
-
-
-    if type(q) != type(None):
-        q.put(0)
-
-    return df
-
-            
-        
-        
-        
-                
-        
-    
-     
+import numpy as np
+import pandas as pd
+import scipy.stats as stats
+import os
+import uuid
+import bisect
+from . import printProgressBar, startConcurrentTask, getIndexOfClosestValue
+from sklearn.ensemble import RandomForestRegressor
+import matplotlib.pyplot as plt
+
+
+class PeakList():
+    def __init__(self,peakList = None):
+        if type(peakList) == type(None):
+            self.peakList = pd.DataFrame()
+        else:
+            self.peakList = peakList
+            
+    def from_df(self,df,sampleCols=None):
+        self.peakList = df
+        if sampleCols is None: self.sampleCols = [x for x in self.peakList.columns.values if x not in ["mz","rt","rt_start","rt_end","isotope","adduct","peak group"]]
+        else: self.sampleCols = sampleCols
+
+    def to_csv(self,fn):
+        self.peakList.to_csv(fn)
+
+    def to_skyline(self,fn,polarity,moleculeListName = "XCMS peaks"):
+        transitionList = pd.DataFrame(self.peakList)
+        transitionList["Precursor Name"] = ["unknown " + str(index) for index, row in transitionList.iterrows()]
+        transitionList["Explicit Retention Time"] = [row["rt_start"] / 2 + row["rt_end"] / 2 for index, row in
+                                                     transitionList.iterrows()]
+        polMapper = {"Positive": 1, "Negative": -1}
+        transitionList["Precursor Charge"] = [polMapper[polarity] for index, row in transitionList.iterrows()]
+        transitionList["Precursor m/z"] = [row["mz"] for index,row in transitionList.iterrows()]
+        transitionList["Molecule List Name"] = [moleculeListName for _ in range(len(transitionList))]
+        transitionList = transitionList[
+            ["Molecule List Name", "Precursor Name", "Precursor m/z", "Precursor Charge",
+             "Explicit Retention Time"]]
+        transitionList.to_csv(fn)
+
+
+
+    def readXCMSPeakList(self,filename,key=".mzML"):
+        data = pd.read_csv(filename,index_col=0,sep="\t")
+        data_form = {}
+        self.sampleCols = [x for x in data.columns.values if key in x]
+        for col in self.sampleCols:
+            data[col] = data[col].fillna(0)
+        for index,row in data.iterrows():
+            data_form[index] = {"mz":row["mzmed"],"rt":row["rtmed"]/60,"rt_start":row["rtmin"]/60,"rt_end":row["rtmax"]/60}#,"isotope_xcms":row["isotopes"],"adduct_xcms":row["adduct"],"peak group":row["pcgroup"]}
+            for col in self.sampleCols:
+               data_form[index][col] = row[col]
+               
+        self.peakList = pd.DataFrame.from_dict(data_form,orient="index")
+
+    def runXCMS(self, path, fn, polarity, ppm, peakWidth,noise=1000,s2n=1,prefilter = 2,mzDiff=0.0001,minFrac=0.0):
+        dir = os.path.dirname(__file__)
+        os.system("Rscript " + os.path.join(dir, "find_peaks.R") + " " + path + " " + polarity + " " + str(
+            ppm) + " " + str(peakWidth[0]) + " " + str(peakWidth[1]) + " " + fn + " " + str(noise) + " " + str(s2n) + " " + str(prefilter) + " " + str(mzDiff) + " " + str(minFrac))
+        self.readXCMSPeakList(path + fn)
+
+    def installRPackages(self):
+        dir = os.path.dirname(__file__)
+        os.system("Rscript " + os.path.join(dir, "install_R_packages.R"))
+
+    #def filterAdductsIsotopes(self,adductsToKeep = ["[M+H]","[M-H]"],isotopesToKeep = ["[M]"]):
+    #    goodRows = []
+    #    for index,row in self.peakList.iterrows():
+    #        if (pd.isna(row["adduct_xcms"]) or any(x in row["adduct_xcms"] for x in adductsToKeep)) and (pd.isna(row["isotope_xcms"]) or any(x in row["isotope_xcms"] for x in isotopesToKeep)):
+    #            goodRows.append(index)
+    #    self.peakList = self.peakList.loc[goodRows,:]
+
+    def removeRedundancy(self,corrThresh,rtThresh,polarity,ppm,numCores,sampleCols=None):
+
+        if sampleCols is None:
+            sampleCols = self.sampleCols
+
+        groups = []
+        anchors = []
+        rts = []
+        c = 0
+
+        self.peakList = self.peakList.sort_values(by="rt",ascending=True)
+        for index,row in self.peakList.iterrows():
+            unique = True
+            if len(rts) > 0:
+                iC = len(rts) - 1
+                rt, vec = anchors[iC]
+
+                if np.abs(rts[iC]-row["rt"]) < rtThresh:
+                    if len(sampleCols) > 2:
+                        r, p = stats.pearsonr(vec, row[sampleCols].values)
+                        if r > corrThresh:
+                            unique = False
+                            groups[iC].append(index)
+                    else:
+                        unique = False
+                        groups[iC].append(index)
+
+            if unique:
+                rts.append(row["rt"])
+                groups.append([index])
+                anchors.append([row["rt"],row[sampleCols].values])
+            c += 1
+            printProgressBar(c,len(self.peakList),prefix="grouping peaks",suffix=str(len(groups)) + " peak groups found",printEnd="")
+
+        self.peakList = self.peakList.sort_index()
+        args = []
+        for i,g in enumerate(groups):
+            filt = self.peakList.loc[g,:]
+            args.append([filt,polarity,ppm])
+        result = startConcurrentTask(runMzUnity,args,numCores,"running mz.unity",len(groups))
+        self.peakList["uniqueIon"] = True
+        for res,g in zip(result,groups):
+            self.peakList.loc[g,res.columns.values] = res.values
+
+        featsRemoved =  len(self.peakList) - len(self.peakList[self.peakList["uniqueIon"]])
+        self.peakList = self.peakList[self.peakList["uniqueIon"]]
+        print(featsRemoved,"redundant features found")
+
+    def backgroundSubtract(self,blank_keys,sample_keys,factor=3):
+        goodRows = []
+        sampleCols = [x for x in self.sampleCols if any(y in x for y  in sample_keys)]
+        blankCols = [x for x in self.sampleCols if any(y in x for y  in blank_keys) and x not in sampleCols]
+        for index,row in self.peakList.iterrows():
+            blankInt = np.mean(row[blankCols])
+            sampleInt = np.mean(row[sampleCols])
+            if sampleInt >= factor * blankInt:
+                goodRows.append(index)
+        print(len(self.peakList)-len(goodRows), "background features found")
+        self.peakList = self.peakList.loc[goodRows,:]
+
+    def imputeRowMin(self,sample_keys,minimum=1):
+
+        arr = self.peakList[sample_keys].values.transpose()
+
+        # find the minimum non-zero value of each compound
+        max_vals = []
+
+        for c in arr.transpose():
+            tmp = [x for x in c if x > minimum]
+            if len(tmp) > 0:
+                max_vals.append(np.min(tmp))
+            else:
+                max_vals.append(2)
+
+        # impute values
+        data_imp = np.zeros(arr.shape)
+        numImputted = 0
+        numNon = 0
+
+        for c in range(arr.shape[1]):
+            for r in range(arr.shape[0]):
+                # if not a missing value
+                if arr[r, c] > 1e-3:
+                    data_imp[r, c] = arr[r, c]
+                    numNon += 1
+                # if it is a missing value
+                else:
+                    data_imp[r, c] = max_vals[c] / 2
+                    numImputted += 1
+        print(numImputted / (numImputted + numNon), "of values imputted")
+
+
+        self.peakList[sample_keys] = data_imp.transpose()
+
+    def logTransform(self,sampleCols):
+        self.peakList[sampleCols] = np.log2(self.peakList[sampleCols].values)
+
+    def batchCorrect(self,sampleCols,qcCols,batchInfo,plot=True):
+
+        reg = RandomForestRegressor(n_jobs=10)
+
+        peak_areas = self.peakList[sampleCols].values.transpose()
+
+        X = np.array(batchInfo[qcCols])
+        y = peak_areas[qcCols] - np.mean(peak_areas[qcCols], axis=0)
+        reg.fit(X, y)
+        preds = reg.predict(batchInfo)
+        if plot:
+            plt.figure()
+            plt.plot(list(range(len(preds))),np.mean(preds,axis=1))
+            plt.errorbar(list(range(len(preds))),np.mean(preds,axis=1),yerr=np.std(preds,axis=1),fmt=".",capsize=1)
+            plt.xlabel("run order")
+            plt.ylabel("correction factor")
+        self.peakList[sampleCols] = np.array(peak_areas - preds).transpose()
+
+        
+
+def compareRT(feat1,feat2,rtTol):
+
+    rt1 = feat1["rt"]
+    rt2 = feat2["rt"]
+    
+    if np.abs(rt1-rt2) < rtTol:
+        return True
+        
+    return False
+
+def mergePeakLists(peakLists,names,ppm=20,rtTol=.5):
+    peakLists = [x[["mz","rt"]].reset_index() for x in peakLists]
+    mergedList = peakLists[0]
+    peakFounders = {n:{} for n in names}
+    peakIndices = {n:{} for n in names}
+
+    for index,row in mergedList.iterrows():
+        peakFounders[names[0]][index] = 1
+        peakIndices[names[0]][index] = index
+        for n in names[1:]:
+            peakFounders[n][index] = 0
+            peakIndices[n][index] = -1
+    for x,n in zip(peakLists[1:],names[1:]):
+        for index,row in x.iterrows():
+            new = True
+            mz_bounds = [row["mz"] - ppm*row["mz"]/1e6,row["mz"] + ppm*row["mz"]/1e6]
+            if len(mergedList) > 0:
+                filt = mergedList[(mergedList["mz"] > mz_bounds[0]) & (mergedList["mz"] < mz_bounds[1])]            
+                for index2,row2 in filt.iterrows():
+                    if compareRT(row,row2,rtTol):
+                        new = False
+                        peakFounders[n][index2] = 1
+                        peakIndices[n][index2] = index
+                        break
+            if new:
+                ind = len(mergedList)
+                mergedList = pd.concat((mergedList,x.iloc[index:index+1,:]),axis=0,ignore_index=True)
+                for n2 in names:
+                    peakFounders[n2][ind] = 0
+                    peakIndices[n2][ind] = -1
+
+                peakFounders[n][ind] = 1
+                peakIndices[n][ind] = index
+                
+      
+                            
+    peakFounders = pd.DataFrame.from_dict(peakFounders,orient="index").transpose()
+    peakIndices = pd.DataFrame.from_dict(peakIndices,orient="index").transpose()
+
+    return pd.concat((mergedList,peakFounders),axis=1,ignore_index=False),pd.concat((mergedList,peakIndices),axis=1,ignore_index=False)
+
+def runMzUnity(df,polarity,ppm,q=None):
+    dir = os.path.dirname(__file__)
+    path = str(uuid.uuid4()) + ".csv"
+    if len(df) > 1:
+        df.to_csv(path)
+        os.system("Rscript " + os.path.join(dir, "mz_unity.R") + " " + path + " " + str(polarity) + " " + str(ppm) + " " + path)
+        df = pd.read_csv(path,index_col=0)
+        if "uniqueIon" not in df.columns.values:
+            print("bad",len(df))
+            df["uniqueIon"] = True
+        else:
+            os.remove(path)
+
+    else:
+        df["uniqueIon"] = True
+
+    #check for duplicate mzs
+    mzs = df["mz"].values
+    for x in range(len(mzs)):
+        for y in range(x):
+            if abs(mzs[x] - mzs[y])/mzs[x] < ppm:
+                df.at[df.index.values[y],"uniqueIon"] = False
+
+
+
+
+    if type(q) != type(None):
+        q.put(0)
+
+    return df
+
+            
+        
+        
+        
+                
+        
+    
+
```

### Comparing `PeakDetective-0.1.6/PeakDetective/find_peaks.R` & `PeakDetective-0.1.8/PeakDetective/find_peaks.R`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-library("xcms")
-#library("CAMERA")
-
-args = commandArgs(trailingOnly=TRUE)
-
-pathData <- args[1] #path to your .mzML
-charge <- args[2]
-ppm <- as.numeric(args[3])
-minWidth <- as.numeric(args[4])
-maxWidth <- as.numeric(args[5])
-noise <- as.numeric(args[7])#1
-s2n <- as.numeric(args[8])#14.14
-prefilter <- as.numeric(args[9])#1
-mzDiff <- as.numeric(args[10])#.0001
-frac <- as.numeric(args[11])
-fn <- args[6]
-
-register(SerialParam())
-
-
-setwd(pathData)
-
-files = list.files(pattern = "*.mzML")
-
-numFiles = length(files)
-
-xs = readMSData(files,mode="onDisk",msLevel=1)
-
-xs = filterEmptySpectra(xs)
-
-params <- CentWaveParam(ppm = ppm, peakwidth = c(minWidth, maxWidth),noise=noise,
-                        snthresh = s2n,mzdiff = mzDiff,prefilter = c(prefilter,100),
-                        mzCenterFun = "wMean",integrate = 1,fitgauss = FALSE,verboseColumns = FALSE)
-
-xs2 <- findChromPeaks(xs,params,return.type="XCMSnExp")
-
-pdp <- PeakDensityParam(sampleGroups = rep(1,numFiles),
-                        minFraction = frac,bw=2)
-
-xs2 = groupChromPeaks(xs2,param=pdp)
-
-
-xs2 = adjustRtime(xs2, ObiwarpParam(binSize = 1,))
-
-xs2 = groupChromPeaks(xs2,param=pdp)
-
-xs3 = fillChromPeaks(xs2)
-
-#format results
-peakInfo = featureDefinitions(xs3)
-intensities = featureValues(xs3)
-peaktable = merge(peakInfo, intensities,
-                          by = 'row.names', all = TRUE)
-
-#write output
-drop <- c("peakidx")
-write.table(peaktable[,!(names(peaktable) %in% drop)],fn,sep="\t",row.names=FALSE,col.names=TRUE)
-
-
-#xs3 = xs2
-
-#xs4 = as(xs3, "xcmsSet")
-
-#ann = annotate(xs4,polarity=charge,maxcharge=2,ppm=ppm)
-
-#peaks = getPeaklist(ann)
-
-#write.csv(peaks,fn)
+library("xcms")
+#library("CAMERA")
+
+args = commandArgs(trailingOnly=TRUE)
+
+pathData <- args[1] #path to your .mzML
+charge <- args[2]
+ppm <- as.numeric(args[3])
+minWidth <- as.numeric(args[4])
+maxWidth <- as.numeric(args[5])
+noise <- as.numeric(args[7])#1
+s2n <- as.numeric(args[8])#14.14
+prefilter <- as.numeric(args[9])#1
+mzDiff <- as.numeric(args[10])#.0001
+frac <- as.numeric(args[11])
+fn <- args[6]
+
+register(SerialParam())
+
+
+setwd(pathData)
+
+files = list.files(pattern = "*.mzML")
+
+numFiles = length(files)
+
+xs = readMSData(files,mode="onDisk",msLevel=1)
+
+xs = filterEmptySpectra(xs)
+
+params <- CentWaveParam(ppm = ppm, peakwidth = c(minWidth, maxWidth),noise=noise,
+                        snthresh = s2n,mzdiff = mzDiff,prefilter = c(prefilter,100),
+                        mzCenterFun = "wMean",integrate = 1,fitgauss = FALSE,verboseColumns = FALSE)
+
+xs2 <- findChromPeaks(xs,params,return.type="XCMSnExp")
+
+pdp <- PeakDensityParam(sampleGroups = rep(1,numFiles),
+                        minFraction = frac,bw=2)
+
+xs2 = groupChromPeaks(xs2,param=pdp)
+
+
+xs2 = adjustRtime(xs2, ObiwarpParam(binSize = 1,))
+
+xs2 = groupChromPeaks(xs2,param=pdp)
+
+xs3 = fillChromPeaks(xs2)
+
+#format results
+peakInfo = featureDefinitions(xs3)
+intensities = featureValues(xs3)
+peaktable = merge(peakInfo, intensities,
+                          by = 'row.names', all = TRUE)
+
+#write output
+drop <- c("peakidx")
+write.table(peaktable[,!(names(peaktable) %in% drop)],fn,sep="\t",row.names=FALSE,col.names=TRUE)
+
+
+#xs3 = xs2
+
+#xs4 = as(xs3, "xcmsSet")
+
+#ann = annotate(xs4,polarity=charge,maxcharge=2,ppm=ppm)
+
+#peaks = getPeaklist(ann)
+
+#write.csv(peaks,fn)
```

### Comparing `PeakDetective-0.1.6/PeakDetective/mz_unity.R` & `PeakDetective-0.1.8/PeakDetective/mz_unity.R`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-library(mz.unity)
-library(dplyr)
-
-args = commandArgs(trailingOnly=TRUE)
-
-inputPath <- args[1]
-outPath <- args[4]
-polarity <- as.integer(args[2])
-ppm <- as.numeric(args[3])
-
-#load data
-mz = read.csv(inputPath)
-
-#format data
-cols = colnames(mz)
-mz$m = mz$mz
-mz$z = polarity
-mz$d = 1
-mz$id = seq(nrow(mz))
-mz$row = seq(nrow(mz))
-
-#gather z=2 ions
-mz2 = mz
-mz2$m = mz2$m * 2
-mz2$z = mz2$z * 2
-
-doubleCharged = mz.unity.search(A = mz2, 
-                        B = mz2, 
-                        M = M.iso, ppm = ppm, 
-                        BM.limits = cbind(M.min = c(1), M.max = c(1), B.n = c(1)))
-
-
-doubleCharged = reindex(doubleCharged, '^A$|^A.|^B$|^B.', mz2$row)
-
-doubleCharged = unique(c(doubleCharged$A,doubleCharged$B.1))
-
-#filter out single charged
-singleCharged = mz[which(!mz$row %in% doubleCharged),]
-
-if (nrow(singleCharged) > 1){
-  #find M+1 ions
-  m1Ions = mz.unity.search(A = singleCharged,
-                         B = singleCharged,
-                         M = M.iso, ppm = ppm,
-                         BM.limits = cbind(M.min = c(1), M.max = c(1), B.n = c(1)))
-
-  m1Ions = reindex(m1Ions,'^A$|^A.|^B$|^B.', singleCharged$row)
-
-  m1Ions = unique(m1Ions$B.1)
-
-  #filterOutM1Ions
-  mIons = singleCharged[which(singleCharged$row %in% m1Ions),]
-
-  if (nrow(mIons) > 1){
-     #find neutral loses
-    nls = mz.unity.search(A = mIons,
-                          B = mIons,
-                          M = M.n, ppm = ppm,
-                          BM.limits = cbind(M.min = c(1), M.max = c(1), B.n = c(1))
-    )
-    nls = reindex(nls,'^A$|^A.|^B$|^B.', mIons$row)
-    nls = unique(nls$A)
-
-    #filter nuetral lose
-    uniqueIons = mIons[which(!mIons$row %in% nls),]
-  }else{
-    uniqueIons = mIons
-  }
-
-
-}else{
-  uniqueIons = singleCharged
-}
-
-
-
-mz$uniqueIon = mz$row %in% uniqueIons$row
-
-
-#filter cols
-mz = mz[,c(cols,"uniqueIon")]
-
-write.csv(mz,outPath,row.names=FALSE)
-
-
-
-
-
-
-
-
-
+library(mz.unity)
+library(dplyr)
+
+args = commandArgs(trailingOnly=TRUE)
+
+inputPath <- args[1]
+outPath <- args[4]
+polarity <- as.integer(args[2])
+ppm <- as.numeric(args[3])
+
+#load data
+mz = read.csv(inputPath)
+
+#format data
+cols = colnames(mz)
+mz$m = mz$mz
+mz$z = polarity
+mz$d = 1
+mz$id = seq(nrow(mz))
+mz$row = seq(nrow(mz))
+
+#gather z=2 ions
+mz2 = mz
+mz2$m = mz2$m * 2
+mz2$z = mz2$z * 2
+
+doubleCharged = mz.unity.search(A = mz2, 
+                        B = mz2, 
+                        M = M.iso, ppm = ppm, 
+                        BM.limits = cbind(M.min = c(1), M.max = c(1), B.n = c(1)))
+
+
+doubleCharged = reindex(doubleCharged, '^A$|^A.|^B$|^B.', mz2$row)
+
+doubleCharged = unique(c(doubleCharged$A,doubleCharged$B.1))
+
+#filter out single charged
+singleCharged = mz[which(!mz$row %in% doubleCharged),]
+
+if (nrow(singleCharged) > 1){
+  #find M+1 ions
+  m1Ions = mz.unity.search(A = singleCharged,
+                         B = singleCharged,
+                         M = M.iso, ppm = ppm,
+                         BM.limits = cbind(M.min = c(1), M.max = c(1), B.n = c(1)))
+
+  m1Ions = reindex(m1Ions,'^A$|^A.|^B$|^B.', singleCharged$row)
+
+  m1Ions = unique(m1Ions$B.1)
+
+  #filterOutM1Ions
+  mIons = singleCharged[which(singleCharged$row %in% m1Ions),]
+
+  if (nrow(mIons) > 1){
+     #find neutral loses
+    nls = mz.unity.search(A = mIons,
+                          B = mIons,
+                          M = M.n, ppm = ppm,
+                          BM.limits = cbind(M.min = c(1), M.max = c(1), B.n = c(1))
+    )
+    nls = reindex(nls,'^A$|^A.|^B$|^B.', mIons$row)
+    nls = unique(nls$A)
+
+    #filter nuetral lose
+    uniqueIons = mIons[which(!mIons$row %in% nls),]
+  }else{
+    uniqueIons = mIons
+  }
+
+
+}else{
+  uniqueIons = singleCharged
+}
+
+
+
+mz$uniqueIon = mz$row %in% uniqueIons$row
+
+
+#filter cols
+mz = mz[,c(cols,"uniqueIon")]
+
+write.csv(mz,outPath,row.names=FALSE)
+
+
+
+
+
+
+
+
+
```

### Comparing `PeakDetective-0.1.6/setup.py` & `PeakDetective-0.1.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from setuptools import setup, find_packages
-
-setup(
-    name='PeakDetective',  # How you named your package folder (MyLib)
-    packages=["PeakDetective"],  # Chose the same as "name"
-    version='0.1.6',  # Start with a small number and increase it with every change you make
-    license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
-    description='Curates and detects LC/MS peaks in metabolomics datasets',  # Give a short description about your library
-    author='Ethan Stancliffe',  # Type in your name
-    author_email='estancl1234@gmail.com',  # Type in your E-Mail
-    url='https://github.com/e-stan/PeakDetective/',  # Provide either the link to your github or to your website
-    download_url='https://github.com/e-stan/PeakDetective/archive/v0.1.6.tar.gz',  # I explain this later on
-    keywords=['Metabolomics', 'LC/MS', "Deep Learning","semi-supervised learning","machine learning"],  # Keywords that define your package best
-    install_requires=[  # I get to this in a second
-        'pyteomics',
-        'numpy',
-        'scipy',
-        "matplotlib",
-        "tensorflow",
-        "scikit-learn",
-        "fastdtw"
-    ],
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
-        'Intended Audience :: Developers',  # Define that your audience are developers
-        'Topic :: Software Development :: Build Tools',
-        'License :: OSI Approved :: MIT License',  # Again, pick a license
-        'Programming Language :: Python :: 3.7',  # Specify which pyhton versions that you want to support
-    ],
-    package_data={
-        "": ["*.R"]
-    }
+from setuptools import setup, find_packages
+
+setup(
+    name='PeakDetective',  # How you named your package folder (MyLib)
+    packages=["PeakDetective"],  # Chose the same as "name"
+    version='0.1.8',  # Start with a small number and increase it with every change you make
+    license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
+    description='Curates and detects LC/MS peaks in metabolomics datasets',  # Give a short description about your library
+    author='Ethan Stancliffe',  # Type in your name
+    author_email='estancl1234@gmail.com',  # Type in your E-Mail
+    url='https://github.com/e-stan/PeakDetective/',  # Provide either the link to your github or to your website
+    download_url='https://github.com/e-stan/PeakDetective/archive/v0.1.8.tar.gz',  # I explain this later on
+    keywords=['Metabolomics', 'LC/MS', "Deep Learning","semi-supervised learning","machine learning"],  # Keywords that define your package best
+    install_requires=[  # I get to this in a second
+        'pyteomics',
+        'numpy',
+        'scipy',
+        "matplotlib",
+        "tensorflow",
+        "scikit-learn",
+        "fastdtw"
+    ],
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
+        'Intended Audience :: Developers',  # Define that your audience are developers
+        'Topic :: Software Development :: Build Tools',
+        'License :: OSI Approved :: MIT License',  # Again, pick a license
+        'Programming Language :: Python :: 3.7',  # Specify which pyhton versions that you want to support
+    ],
+    package_data={
+        "": ["*.R"]
+    }
 )
```

