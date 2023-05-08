# Comparing `tmp/DarwinPy-0.0.1.tar.gz` & `tmp/DarwinPy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\DarwinPy-0.0.1.tar", last modified: Sat Oct 16 12:08:00 2021, max compression
+gzip compressed data, was "DarwinPy-0.0.2.tar", last modified: Mon May  8 13:39:34 2023, max compression
```

## Comparing `DarwinPy-0.0.1.tar` & `DarwinPy-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2021-10-16 12:08:00.000000 DarwinPy-0.0.1/
--rw-rw-rw-   0        0        0       83 2021-10-10 12:48:50.000000 DarwinPy-0.0.1/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2021-10-16 12:07:57.000000 DarwinPy-0.0.1/DarwinPy/
-drwxrwxrwx   0        0        0        0 2021-10-16 12:07:59.000000 DarwinPy-0.0.1/DarwinPy/Core/
--rw-rw-rw-   0        0        0      197 2021-08-16 14:49:52.000000 DarwinPy-0.0.1/DarwinPy/Core/__init__.py
-drwxrwxrwx   0        0        0        0 2021-10-16 12:07:59.000000 DarwinPy-0.0.1/DarwinPy/EvolutionaryStrategy/
--rw-rw-rw-   0        0        0     5019 2021-08-10 20:21:38.000000 DarwinPy-0.0.1/DarwinPy/EvolutionaryStrategy/__init__.py
-drwxrwxrwx   0        0        0        0 2021-10-16 12:07:59.000000 DarwinPy-0.0.1/DarwinPy/Functions/
--rw-rw-rw-   0        0        0      436 2021-08-11 06:05:40.000000 DarwinPy-0.0.1/DarwinPy/Functions/__init__.py
-drwxrwxrwx   0        0        0        0 2021-10-16 12:08:00.000000 DarwinPy-0.0.1/DarwinPy/Genetics/
--rw-rw-rw-   0        0        0     3958 2021-09-17 13:19:08.000000 DarwinPy-0.0.1/DarwinPy/Genetics/__init__.py
-drwxrwxrwx   0        0        0        0 2021-10-16 12:08:00.000000 DarwinPy-0.0.1/DarwinPy/Utils/
--rw-rw-rw-   0        0        0      260 2021-08-26 17:51:41.000000 DarwinPy-0.0.1/DarwinPy/Utils/__init__.py
--rw-rw-rw-   0        0        0     3224 2021-10-16 10:23:59.000000 DarwinPy-0.0.1/DarwinPy/__init__.py
-drwxrwxrwx   0        0        0        0 2021-10-16 12:07:58.000000 DarwinPy-0.0.1/DarwinPy.egg-info/
--rw-rw-rw-   0        0        0     2897 2021-10-16 12:07:50.000000 DarwinPy-0.0.1/DarwinPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2021-10-16 12:07:51.000000 DarwinPy-0.0.1/DarwinPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-16 12:07:50.000000 DarwinPy-0.0.1/DarwinPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2021-10-16 12:07:50.000000 DarwinPy-0.0.1/DarwinPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2021-10-16 12:07:50.000000 DarwinPy-0.0.1/DarwinPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       27 2021-10-10 13:05:38.000000 DarwinPy-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2897 2021-10-16 12:08:00.000000 DarwinPy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1681 2021-10-16 10:28:33.000000 DarwinPy-0.0.1/README.md
--rw-rw-rw-   0        0        0       14 2021-09-28 16:22:49.000000 DarwinPy-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2021-10-16 12:08:00.000000 DarwinPy-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      753 2021-10-16 12:05:55.000000 DarwinPy-0.0.1/setup.py
--rw-rw-rw-   0        0        0     1562 2021-10-08 15:29:43.000000 DarwinPy-0.0.1/test.py
--rw-rw-rw-   0        0        0      219 2021-08-11 15:28:43.000000 DarwinPy-0.0.1/todo.txt
+drwxr-xr-x   0 pius       (502) staff       (20)        0 2023-05-08 13:39:34.487950 DarwinPy-0.0.2/
+-rw-r--r--   0 pius       (502) staff       (20)       77 2023-05-08 12:54:09.000000 DarwinPy-0.0.2/CHANGELOG.txt
+drwxr-xr-x   0 pius       (502) staff       (20)        0 2023-05-08 13:39:34.485429 DarwinPy-0.0.2/DarwinPy/
+drwxr-xr-x   0 pius       (502) staff       (20)        0 2023-05-08 13:39:34.486810 DarwinPy-0.0.2/DarwinPy/Core/
+-rw-r--r--   0 pius       (502) staff       (20)      186 2023-05-08 12:54:09.000000 DarwinPy-0.0.2/DarwinPy/Core/__init__.py
+drwxr-xr-x   0 pius       (502) staff       (20)        0 2023-05-08 13:39:34.486997 DarwinPy-0.0.2/DarwinPy/EvolutionaryStrategy/
+-rw-r--r--   0 pius       (502) staff       (20)     4859 2023-05-08 12:54:09.000000 DarwinPy-0.0.2/DarwinPy/EvolutionaryStrategy/__init__.py
+drwxr-xr-x   0 pius       (502) staff       (20)        0 2023-05-08 13:39:34.487192 DarwinPy-0.0.2/DarwinPy/Functions/
+-rw-r--r--   0 pius       (502) staff       (20)      424 2023-05-08 12:54:09.000000 DarwinPy-0.0.2/DarwinPy/Functions/__init__.py
+drwxr-xr-x   0 pius       (502) staff       (20)        0 2023-05-08 13:39:34.487354 DarwinPy-0.0.2/DarwinPy/Genetics/
+-rw-r--r--   0 pius       (502) staff       (20)     3816 2023-05-08 12:54:09.000000 DarwinPy-0.0.2/DarwinPy/Genetics/__init__.py
+drwxr-xr-x   0 pius       (502) staff       (20)        0 2023-05-08 13:39:34.487529 DarwinPy-0.0.2/DarwinPy/Utils/
+-rw-r--r--   0 pius       (502) staff       (20)      242 2023-05-08 12:54:09.000000 DarwinPy-0.0.2/DarwinPy/Utils/__init__.py
+-rw-r--r--   0 pius       (502) staff       (20)     3140 2023-05-08 12:54:09.000000 DarwinPy-0.0.2/DarwinPy/__init__.py
+drwxr-xr-x   0 pius       (502) staff       (20)        0 2023-05-08 13:39:34.486666 DarwinPy-0.0.2/DarwinPy.egg-info/
+-rw-r--r--   0 pius       (502) staff       (20)     4921 2023-05-08 13:39:34.000000 DarwinPy-0.0.2/DarwinPy.egg-info/PKG-INFO
+-rw-r--r--   0 pius       (502) staff       (20)      422 2023-05-08 13:39:34.000000 DarwinPy-0.0.2/DarwinPy.egg-info/SOURCES.txt
+-rw-r--r--   0 pius       (502) staff       (20)        1 2023-05-08 13:39:34.000000 DarwinPy-0.0.2/DarwinPy.egg-info/dependency_links.txt
+-rw-r--r--   0 pius       (502) staff       (20)        6 2023-05-08 13:39:34.000000 DarwinPy-0.0.2/DarwinPy.egg-info/requires.txt
+-rw-r--r--   0 pius       (502) staff       (20)        9 2023-05-08 13:39:34.000000 DarwinPy-0.0.2/DarwinPy.egg-info/top_level.txt
+-rw-r--r--   0 pius       (502) staff       (20)     1073 2023-05-08 12:54:09.000000 DarwinPy-0.0.2/LICENSE
+-rw-r--r--   0 pius       (502) staff       (20)       26 2023-05-08 12:54:09.000000 DarwinPy-0.0.2/MANIFEST.in
+-rw-r--r--   0 pius       (502) staff       (20)     4921 2023-05-08 13:39:34.487798 DarwinPy-0.0.2/PKG-INFO
+-rw-r--r--   0 pius       (502) staff       (20)     4279 2023-05-08 13:00:44.000000 DarwinPy-0.0.2/README.md
+-rw-r--r--   0 pius       (502) staff       (20)       14 2023-05-08 12:54:09.000000 DarwinPy-0.0.2/requirements.txt
+-rw-r--r--   0 pius       (502) staff       (20)       38 2023-05-08 13:39:34.487997 DarwinPy-0.0.2/setup.cfg
+-rw-r--r--   0 pius       (502) staff       (20)      727 2023-05-08 13:39:28.000000 DarwinPy-0.0.2/setup.py
+-rw-r--r--   0 pius       (502) staff       (20)     1446 2023-05-08 13:00:08.000000 DarwinPy-0.0.2/test.py
+-rw-r--r--   0 pius       (502) staff       (20)      214 2023-05-08 12:54:09.000000 DarwinPy-0.0.2/todo.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `DarwinPy-0.0.1/DarwinPy/EvolutionaryStrategy/__init__.py` & `DarwinPy-0.0.2/DarwinPy/EvolutionaryStrategy/__init__.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,160 +1,160 @@
-import random #{temporary random}
-import numpy as np
-
-
-class EvolutionaryStrategy:
-	vector_length = 0
-	search_space = ()
-	parent_matrix = []
-	children_matrix = []
-	parent_population_size = 0
-	children_population_size = 0
-	data_type = 0
-
-	def __init__(self,vector_length,parent_population_size,children_population_size,search_space,data_type):
-	    self.vector_length = vector_length
-	    self.search_space = search_space
-	    self.parent_population_size = parent_population_size
-	    self.children_population_size = children_population_size; self.data_type = data_type
-
-
-	def generateParent(self):
-		parent_matrix = np.array(
-		range(self.vector_length * self.parent_population_size), self.data_type).reshape(
-		self.parent_population_size, self.vector_length
-		)
-		for i in range(self.parent_population_size):
-			temp = []
-			for j in range(self.vector_length):
-				rand = random.randint(self.search_space[0],
-				self.search_space[1])
-				parent_matrix[i][j] = rand
-		self.parent_matrix = parent_matrix
-
-
-	def generateOffspring(self, mutation_rate, parent_fitness):
-		children_matrix = np.array(
-		range(self.vector_length * self.children_population_size), self.data_type).reshape(
-		self.children_population_size, self.vector_length
-		)
-		for i in range(self.children_population_size):
-			children_matrix[i] = self.mutate(self.selectParent(parent_fitness),mutation_rate)
-		self.children_matrix = children_matrix
-
-
-	# def generateOffspring(self, parent_fitness, mutation_rate):
-	# 	pass
-
-
-	def mutate(self,vector, mutation_rate):
-		mutant = vector.copy()
-		for i in range(len(vector)):
-			rand = random.random()
-			if rand < mutation_rate:
-				if self.data_type == float:
-					mutant[i] = random.uniform(self.search_space[0],
-					self.search_space[1])
-				elif self.data_type == int:
-					mutant[i] = random.randint(self.search_space[0],
-					self.search_space[1])
-		return mutant
-
-
-	def selectParent(self,parent_fitness):
-		fitness_vector_sum = parent_fitness.sum()
-		parent_fitness_prob = parent_fitness.copy()
-		if fitness_vector_sum == 0:
-			for i in range(len(parent_fitness)):
-				parent_fitness_prob[i] = 1/len(parent_fitness)
-		else:
-			for i in range(len(parent_fitness)):
-				parent_fitness_prob[i] = parent_fitness[i]/fitness_vector_sum
-		rand = random.random()
-		j = 0
-		while rand > 0:
-			rand -= parent_fitness_prob[j]
-			j += 1
-		if j == 0:
-			return self.parent_matrix[0]
-		else:
-			j -= 1
-			return self.parent_matrix[j]
-
-
-	def  evaluateParent(self,fitness_vector):
-		pass
-
-
-	def getFitness(self):
-		pass
-
-
-	def evaluateChildren(self,fitness_vector):
-		pass
-
-
-	def selectNextGeneration(self,parent_fitness,children_fitness):
-		temp_1 = [[0]*self.vector_length]*(self.children_population_size +
-		self.parent_population_size)
-		temp_2 = [0]*(self.children_population_size + self.parent_population_size)
-		parent_children_matrix = np.array(temp_1,int)
-		parent_children_fitness = np.array(temp_2,float)
-
-		# print("DEBUG!\nchildren matrix:\n {}\nparent_matrix:\n {}\n".
-		# format(self.children_matrix,self.parent_matrix))
-		for i in range(self.parent_population_size):
-			parent_children_matrix[i] = self.parent_matrix[i]
-
-		j = 0
-		for i in range(self.parent_population_size, self.parent_population_size + self.children_population_size):
-			parent_children_matrix[i] = self.children_matrix[j]
-			j += 1
-
-		for i in range(self.parent_population_size):
-			parent_children_fitness[i] = parent_fitness[i]
-		j = 0
-		for i in range(self.parent_population_size, self.parent_population_size + self.children_population_size):
-			# print("DEBUG!")
-			parent_children_fitness[i] = children_fitness[j]
-			j += 1
-
-		fitness_prob = np.array([0]*(self.parent_population_size + self.children_population_size),
-		float)
-
-		fitness_vector_sum = parent_children_fitness.sum()
-		if fitness_vector_sum == 0:
-			for i in range(self.parent_population_size + self.children_population_size):
-				fitness_prob[i] = 1/self.parent_children_fitness
-		else:
-			for i in range(self.parent_population_size + self.children_population_size):
-				fitness_prob[i] = parent_children_fitness[i]/fitness_vector_sum
-
-		temp_3 = [[0]*self.vector_length]*self.parent_population_size
-		# print("the fitness probability vector: {}".format(fitness_prob))
-		next_generation = np.array(temp_3, self.data_type)
-		for i in range(self.parent_population_size):
-			rand = random.random()
-			j = 0
-			while rand > 0:
-				rand -= fitness_prob[j]
-				j += 1
-			if j != 0:
-				j -= 1
-
-			next_generation[i] = parent_children_matrix[j]
-		self.parent_matrix = next_generation
-
-		# print("parent-children matrix:\n {}".
-		# format(parent_children_matrix))
-
-
-	def evolve(self,children_fitness,parent_fitness):
-		self.selectNextGeneration(children_fitness,parent_fitness)
-
-
-	def getParentGeneration(self):
-		return self.parent_matrix
-
-
-	def getChildrenGeneration(self):
-		return self.children_matrix
+import random #{temporary random}
+import numpy as np
+
+
+class EvolutionaryStrategy:
+	vector_length = 0
+	search_space = ()
+	parent_matrix = []
+	children_matrix = []
+	parent_population_size = 0
+	children_population_size = 0
+	data_type = 0
+
+	def __init__(self,vector_length,parent_population_size,children_population_size,search_space,data_type):
+	    self.vector_length = vector_length
+	    self.search_space = search_space
+	    self.parent_population_size = parent_population_size
+	    self.children_population_size = children_population_size; self.data_type = data_type
+
+
+	def generateParent(self):
+		parent_matrix = np.array(
+		range(self.vector_length * self.parent_population_size), self.data_type).reshape(
+		self.parent_population_size, self.vector_length
+		)
+		for i in range(self.parent_population_size):
+			temp = []
+			for j in range(self.vector_length):
+				rand = random.randint(self.search_space[0],
+				self.search_space[1])
+				parent_matrix[i][j] = rand
+		self.parent_matrix = parent_matrix
+
+
+	def generateOffspring(self, mutation_rate, parent_fitness):
+		children_matrix = np.array(
+		range(self.vector_length * self.children_population_size), self.data_type).reshape(
+		self.children_population_size, self.vector_length
+		)
+		for i in range(self.children_population_size):
+			children_matrix[i] = self.mutate(self.selectParent(parent_fitness),mutation_rate)
+		self.children_matrix = children_matrix
+
+
+	# def generateOffspring(self, parent_fitness, mutation_rate):
+	# 	pass
+
+
+	def mutate(self,vector, mutation_rate):
+		mutant = vector.copy()
+		for i in range(len(vector)):
+			rand = random.random()
+			if rand < mutation_rate:
+				if self.data_type == float:
+					mutant[i] = random.uniform(self.search_space[0],
+					self.search_space[1])
+				elif self.data_type == int:
+					mutant[i] = random.randint(self.search_space[0],
+					self.search_space[1])
+		return mutant
+
+
+	def selectParent(self,parent_fitness):
+		fitness_vector_sum = parent_fitness.sum()
+		parent_fitness_prob = parent_fitness.copy()
+		if fitness_vector_sum == 0:
+			for i in range(len(parent_fitness)):
+				parent_fitness_prob[i] = 1/len(parent_fitness)
+		else:
+			for i in range(len(parent_fitness)):
+				parent_fitness_prob[i] = parent_fitness[i]/fitness_vector_sum
+		rand = random.random()
+		j = 0
+		while rand > 0:
+			rand -= parent_fitness_prob[j]
+			j += 1
+		if j == 0:
+			return self.parent_matrix[0]
+		else:
+			j -= 1
+			return self.parent_matrix[j]
+
+
+	def  evaluateParent(self,fitness_vector):
+		pass
+
+
+	def getFitness(self):
+		pass
+
+
+	def evaluateChildren(self,fitness_vector):
+		pass
+
+
+	def selectNextGeneration(self,parent_fitness,children_fitness):
+		temp_1 = [[0]*self.vector_length]*(self.children_population_size +
+		self.parent_population_size)
+		temp_2 = [0]*(self.children_population_size + self.parent_population_size)
+		parent_children_matrix = np.array(temp_1,int)
+		parent_children_fitness = np.array(temp_2,float)
+
+		# print("DEBUG!\nchildren matrix:\n {}\nparent_matrix:\n {}\n".
+		# format(self.children_matrix,self.parent_matrix))
+		for i in range(self.parent_population_size):
+			parent_children_matrix[i] = self.parent_matrix[i]
+
+		j = 0
+		for i in range(self.parent_population_size, self.parent_population_size + self.children_population_size):
+			parent_children_matrix[i] = self.children_matrix[j]
+			j += 1
+
+		for i in range(self.parent_population_size):
+			parent_children_fitness[i] = parent_fitness[i]
+		j = 0
+		for i in range(self.parent_population_size, self.parent_population_size + self.children_population_size):
+			# print("DEBUG!")
+			parent_children_fitness[i] = children_fitness[j]
+			j += 1
+
+		fitness_prob = np.array([0]*(self.parent_population_size + self.children_population_size),
+		float)
+
+		fitness_vector_sum = parent_children_fitness.sum()
+		if fitness_vector_sum == 0:
+			for i in range(self.parent_population_size + self.children_population_size):
+				fitness_prob[i] = 1/self.parent_children_fitness
+		else:
+			for i in range(self.parent_population_size + self.children_population_size):
+				fitness_prob[i] = parent_children_fitness[i]/fitness_vector_sum
+
+		temp_3 = [[0]*self.vector_length]*self.parent_population_size
+		# print("the fitness probability vector: {}".format(fitness_prob))
+		next_generation = np.array(temp_3, self.data_type)
+		for i in range(self.parent_population_size):
+			rand = random.random()
+			j = 0
+			while rand > 0:
+				rand -= fitness_prob[j]
+				j += 1
+			if j != 0:
+				j -= 1
+
+			next_generation[i] = parent_children_matrix[j]
+		self.parent_matrix = next_generation
+
+		# print("parent-children matrix:\n {}".
+		# format(parent_children_matrix))
+
+
+	def evolve(self,children_fitness,parent_fitness):
+		self.selectNextGeneration(children_fitness,parent_fitness)
+
+
+	def getParentGeneration(self):
+		return self.parent_matrix
+
+
+	def getChildrenGeneration(self):
+		return self.children_matrix
```

### Comparing `DarwinPy-0.0.1/DarwinPy/Genetics/__init__.py` & `DarwinPy-0.0.2/DarwinPy/Genetics/__init__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,142 +1,142 @@
-import random #{temporary random}
-import numpy as np
-
-
-class Genetics:
-	chromosome_length = 0
-	population_size = 0
-	search_space = ()
-	chromosome_matrix = []
-	pair_list = []
-	data_type = 0
-
-
-	def __init__(self,chromosome_length, population_size, search_space, data_type):
-		self.chromosome_length = chromosome_length
-		self.population_size = population_size
-		self.search_space = search_space
-		self.data_type = data_type
-
-
-	def crossover(self, crossover_rate):
-		# print(self.pair_list)
-		temp_chromosome_matrix = []
-		for i in range(self.population_size):
-			temp_chromosome_vector = []
-			for j in range(self.chromosome_length):
-				rand = random.random()
-				if rand < crossover_rate:
-					temp_chromosome_vector.append(
-					self.chromosome_matrix[self.pair_list[i][0]][j])
-				else:
-					temp_chromosome_vector.append(
-					self.chromosome_matrix[self.pair_list[i][1]][j])
-			temp_chromosome_matrix.append(temp_chromosome_vector)
-		self.chromosome_matrix = np.array(temp_chromosome_matrix,int)
-
-
-	# def crossoverSplice(self, crossover_rate):
-	# 	temp_chromosome_matrix = []
-	# 	partition = crossover_rate * self.chromosome_length
-	#
-	# 	for i in range(self.population_size):
-	# 		temp_chromosome_vector = []
-	# 		pass
-	# 	pass
-
-
-	def select(self, fitness_vector):
-		fitness_vector_sum = fitness_vector.sum()
-		self.pair_list=[]
-		fitness_prob = []
-		if fitness_vector_sum == 0:
-			temp_fitness_prob = []
-			for i in range(self.population_size):
-				temp_fitness_prob.append(1/self.population_size)
-			fitness_prob = np.array(temp_fitness_prob,float)
-		else:
-			temp_fitness_prob = []
-			for i in range(self.population_size):
-				temp_fitness_prob.append(fitness_vector[i]/fitness_vector_sum)
-			fitness_prob = np.array(temp_fitness_prob,float)
-		# print("DEBUG!")
-		# print("the fitness vector probability: {}".format(fitness_prob))
-		for i in range(self.population_size):
-			# print("DEBUG! {}".format(i))
-			rand = random.random()
-			j = 0
-			while rand > 0:
-				rand -= fitness_prob[j]
-				j += 1
-			if j != 0:
-				j -= 1
-			rand = random.random()
-			k = 0
-			while rand > 0:
-				rand -= fitness_prob[k]
-				k += 1
-			if k != 0:
-				k -= 1
-			self.pair_list.append((j,k))
-		# print(self.pair_list)
-
-
-	def populate(self):
-		temp_chromosome_matrix = []
-		for i in range(self.population_size):
-			temp=[]
-			for j in range(self.chromosome_length):
-				if self.data_type == int:
-					rand = random.randint(self.search_space[0],
-					self.search_space[1])
-				if self.data_type == float:
-					rand = random.uniform(self.search_space[0],
-					self.search_space[1])
-				temp.append(rand)
-			temp_chromosome_matrix.append(temp)
-		self.chromosome_matrix = np.array(temp_chromosome_matrix,self.data_type)
-
-
-	def mutate(self,mutation_rate):
-		for i in range(self.population_size):
-			mutant=self.chromosome_matrix[i]
-			for j in range(self.chromosome_length):
-				rand=random.random()
-				if rand < mutation_rate:
-					if self.data_type == float:
-						mutant[j] = random.uniform(self.search_space[0],
-						self.search_space[1])
-					if self.data_type == int:
-						mutant[j]=random.randint(self.search_space[0],
-						self.search_space[1])
-		# print(self.chromosome_matrix)
-
-
-	def evolve(self,fitness_vector, mutation_rate, crossover_rate):
-		self.select(fitness_vector)
-		self.crossover(crossover_rate)
-		self.mutate(mutation_rate)
-
-
-	def setSearchSpace(self,search_space):
-		self.search_space = search_space
-
-
-	def setChromosomeLength(self, chromosome_length):
-		self.chromosome_length = chromosome_length
-
-
-	def setPopulationSize(self,population_size):
-		self.population_size = population_size
-
-
-	def setChromosomeMatrix(self,chromosome_matrix):
-		self.chromosome_matrix = chromosome_matrix
-
-
-	def getChromosomeMatrix(self):
-		return self.chromosome_matrix
-
-
-	def getSearchSpace(self):
-		return self.search_space
+import random #{temporary random}
+import numpy as np
+
+
+class Genetics:
+	chromosome_length = 0
+	population_size = 0
+	search_space = ()
+	chromosome_matrix = []
+	pair_list = []
+	data_type = 0
+
+
+	def __init__(self,chromosome_length, population_size, search_space, data_type):
+		self.chromosome_length = chromosome_length
+		self.population_size = population_size
+		self.search_space = search_space
+		self.data_type = data_type
+
+
+	def crossover(self, crossover_rate):
+		# print(self.pair_list)
+		temp_chromosome_matrix = []
+		for i in range(self.population_size):
+			temp_chromosome_vector = []
+			for j in range(self.chromosome_length):
+				rand = random.random()
+				if rand < crossover_rate:
+					temp_chromosome_vector.append(
+					self.chromosome_matrix[self.pair_list[i][0]][j])
+				else:
+					temp_chromosome_vector.append(
+					self.chromosome_matrix[self.pair_list[i][1]][j])
+			temp_chromosome_matrix.append(temp_chromosome_vector)
+		self.chromosome_matrix = np.array(temp_chromosome_matrix,int)
+
+
+	# def crossoverSplice(self, crossover_rate):
+	# 	temp_chromosome_matrix = []
+	# 	partition = crossover_rate * self.chromosome_length
+	#
+	# 	for i in range(self.population_size):
+	# 		temp_chromosome_vector = []
+	# 		pass
+	# 	pass
+
+
+	def select(self, fitness_vector):
+		fitness_vector_sum = fitness_vector.sum()
+		self.pair_list=[]
+		fitness_prob = []
+		if fitness_vector_sum == 0:
+			temp_fitness_prob = []
+			for i in range(self.population_size):
+				temp_fitness_prob.append(1/self.population_size)
+			fitness_prob = np.array(temp_fitness_prob,float)
+		else:
+			temp_fitness_prob = []
+			for i in range(self.population_size):
+				temp_fitness_prob.append(fitness_vector[i]/fitness_vector_sum)
+			fitness_prob = np.array(temp_fitness_prob,float)
+		# print("DEBUG!")
+		# print("the fitness vector probability: {}".format(fitness_prob))
+		for i in range(self.population_size):
+			# print("DEBUG! {}".format(i))
+			rand = random.random()
+			j = 0
+			while rand > 0:
+				rand -= fitness_prob[j]
+				j += 1
+			if j != 0:
+				j -= 1
+			rand = random.random()
+			k = 0
+			while rand > 0:
+				rand -= fitness_prob[k]
+				k += 1
+			if k != 0:
+				k -= 1
+			self.pair_list.append((j,k))
+		# print(self.pair_list)
+
+
+	def populate(self):
+		temp_chromosome_matrix = []
+		for i in range(self.population_size):
+			temp=[]
+			for j in range(self.chromosome_length):
+				if self.data_type == int:
+					rand = random.randint(self.search_space[0],
+					self.search_space[1])
+				if self.data_type == float:
+					rand = random.uniform(self.search_space[0],
+					self.search_space[1])
+				temp.append(rand)
+			temp_chromosome_matrix.append(temp)
+		self.chromosome_matrix = np.array(temp_chromosome_matrix,self.data_type)
+
+
+	def mutate(self,mutation_rate):
+		for i in range(self.population_size):
+			mutant=self.chromosome_matrix[i]
+			for j in range(self.chromosome_length):
+				rand=random.random()
+				if rand < mutation_rate:
+					if self.data_type == float:
+						mutant[j] = random.uniform(self.search_space[0],
+						self.search_space[1])
+					if self.data_type == int:
+						mutant[j]=random.randint(self.search_space[0],
+						self.search_space[1])
+		# print(self.chromosome_matrix)
+
+
+	def evolve(self,fitness_vector, mutation_rate, crossover_rate):
+		self.select(fitness_vector)
+		self.crossover(crossover_rate)
+		self.mutate(mutation_rate)
+
+
+	def setSearchSpace(self,search_space):
+		self.search_space = search_space
+
+
+	def setChromosomeLength(self, chromosome_length):
+		self.chromosome_length = chromosome_length
+
+
+	def setPopulationSize(self,population_size):
+		self.population_size = population_size
+
+
+	def setChromosomeMatrix(self,chromosome_matrix):
+		self.chromosome_matrix = chromosome_matrix
+
+
+	def getChromosomeMatrix(self):
+		return self.chromosome_matrix
+
+
+	def getSearchSpace(self):
+		return self.search_space
```

### Comparing `DarwinPy-0.0.1/setup.py` & `DarwinPy-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from setuptools import setup, find_packages
-
-classifiers = [
-"Development Status :: 5 - Production/Stable",
-"Intended Audience :: Developers",
-"Operating System :: Microsoft :: Windows :: Windows 10",
-"License :: OSI Approved :: MIT License",
-"Programming Language :: Python :: 3"
-]
-
-
-setup(
-name = "DarwinPy",
-version = "0.0.1",
-description = "A evolutionary computation module",
-long_description = open("README.md").read() + "\n\n" + open("CHANGELOG.txt").read(),
-long_description_content_type = "text/markdown",
-url = "",
-author = "Pius Arhanbhunde",
-author_email = "pjacks419@gmail.com",
-license = "MIT License",
-classifiers = classifiers,
-keywords = "evolution",
-packages = find_packages(),
-install_requires = ['numpy']
-)
+from setuptools import setup, find_packages
+
+classifiers = [
+"Development Status :: 5 - Production/Stable",
+"Intended Audience :: Developers",
+"Operating System :: Microsoft :: Windows :: Windows 10",
+"License :: OSI Approved :: MIT License",
+"Programming Language :: Python :: 3"
+]
+
+
+setup(
+name = "DarwinPy",
+version = "0.0.2",
+description = "A evolutionary computation module",
+long_description = open("README.md").read() + "\n\n" + open("CHANGELOG.txt").read(),
+long_description_content_type = "text/markdown",
+url = "",
+author = "Pius Arhanbhunde",
+author_email = "pjacks419@gmail.com",
+license = "MIT License",
+classifiers = classifiers,
+keywords = "evolution",
+packages = find_packages(),
+install_requires = ['numpy']
+)
```

